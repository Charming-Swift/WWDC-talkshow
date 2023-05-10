[WWDC22 Add Live Text interaction to your app](https://developer.apple.com/videos/play/wwdc2022/10026/)
> 작성자: [이다혜](https://github.com/dahae0320)
> 
> 원본: (블로그 주소)
<br>

### 📌 Live Text 

애플이 iOS 버전을 16으로 올리면서 여러가지 기능이 추가되었다. 그 중에 하나가 바로 'Live Text' 기능이다. 이미지에 있는 텍스트를 뽑아주는 아주 편/리/한 기능이다.
Text interactions
Translate
Data detection
QR codes
Live Text는 위에 적은 4개의 기능을 모두 제공한다.

iOS16 버전을 쓰고 있다면, 바로 확인할 수 있다! 사진 앱에서 텍스트가 많은 사진을 살펴보도록 하자.

위 사진처럼 이미지에 있는 텍스트를 자동으로 감지하고, 복사나 선택등의 기능을 수행할 수 있다. 
당연히 번역도 가능하다! 만약 외국에서 글을 읽어야 하는 상황이 온다면(메뉴판이나, 간판 등) 간단히 사진을 찍어서 바로 번역을 할 수 있다. 너무 편리한 기능이다!

그런데 이런 기능을 내가 만든 앱에도 적용할 수 있다? ㅋㅋ당장 알아보도록하자.

<br>

### 📚 Live Text API

사용되는 곳: 이미지, 일시정지된 영상 프레임 (모두 '멈춰'있다는 점)
실시간 카메라 분석으로 해야한다면? Visition Kit의 Capture machine을 다루고 있는 영상을 보면 된다고 한다.
이번 영상에서는 정적인 이미지에 Live Text를 적용하는 방법을 알려주나보다.
iOS 16부터 사용 + Apple Neural Engine, macOS 13.0를 가지는 모든 기기들


어케 쓰냐면
1. 이미지 준비
2. ImageAnalyzer에서 ImageAnalysis
이미지 분석기에서 이미지를 분석한다.
3. 플랫폼에 따라서 ImageAnalysisInteraction, ImageAnalysisOverlayView에 전달된다.

크게 4개의 메인 클래스로 구성되어 있다. 아주 간단한 사용 흐름이다. 

<br>

### 🛠️ Live Text 적용하기

* UIKit을 기준으로 설명하겠습니다.
* ImageAnalysisInteractionDelegate, UIGestureRecognizerDelegate 프로토콜을 채택한 뷰컨 내부에서 작업합니다.

1. ImageAnalyzer, ImageAnalysisInteraction 인스턴스 생성
2. viewDidLoad에
3. 함수 만들기

[ 코드 및 코드 설명 ]

<br>

### 💁🏻‍♀️ Tips and tricks

자! 여기까지 Live Text를 사용하는 흐름에 대해서 살펴보았다. 실제 코드가 어떤지도 알게되었다. 
크게 어렵지 않지만, 개발을 하다보면 원하는데로 흘러가지 않기도 한다. 

코드를 다시 찬찬히 보면서 주의해야할 점들을 알아보자.
1. Preferred interaction types
1-1. ~
- .automatic
- .textSelection
- .dataDetectors
1-2. long press로 텍스트 감지하기 기능 껏켯

2. Supplementary Interface
- Live Text Button
- Quick Actions
- Size and position automatic
Live Text 기능의 인터페이스를 커스텀할 수 있다!
- 인터페이스 안보이게 하기
- 인터페이스 위치 조절하기 (Inset)
- 인터페이스 폰트 변경하기

3. Match highlights to content
UIImageView를 사용하지 않고 다른 방법으로 불러온 Image에 Live Text를 적용한다면, 텍스트의 하이라이트 범위가 이상한 것을 볼 수 있다.
UIImageView를 쓰면 VisitionKit이 알아서 contentRect를 계산해준다. 그게 아니라면.. 제대로 계산이 안된다는거~

4. Interaction placement
Live Text와 상호작용하는 곳을 어디로 두는게 가장 좋을까?
- Over image content
- UIImageView
-> UIImageView안에 ImageAnalysisInteraction을 넣어주도록 하자. 만약 스크롤뷰 안에 이미지뷰가 있다면... 스크롤뷰밖에 놓을 수도 있겠지만, 비추한ㄷ.ㅏ 관리하기 어렵다! (rect가 계속 바뀌므로) 그냥 똑같이 이미지뷰안에 넣자.

5. Gesture Conflict
당연히 라이브 텍스트는 제스처로 상호작용하니까, 다른 제스처가 쓰이고 있다면 충돌이 일어날 수 있다!
어케 바로 잡을 수 있을까?
5-1. 대표적인 방법이 있다.. 바로바로 interactionShouldBeginAtPointForInteractionType (아유 길다)

false를 돌려주면 live text 인터랙션 작동안함.
- 포인트에 인터랙션이 있는 아이템이 있는지 확인하는 것
- 텍스트 선택이 있는지 확인(선택한 텍스트가 아닌 곳을 선택하면 deselect)

5-2. 



5-3. hitText 종료하기



6. 라이브 텍스트를 사용하기 전에 지켜줘야할 점
하나의 이미지분석기만 사용하기
이미지버전 최소화하기
시스템 자원을 최소화하기 위해 이미지가 나타나는 순간이나 그 전에 분석해야 하도록 하자.

7. 다양한 곳에서도 라이브 텍스트가 사용되고 있다.
유아이텍필, 텍뷰, 웹킷, 퀵륵에서도 라이브 텍스트가 사용되고 있다. 자세한 내용은 영상을 보자.

<br>

### ⌗ 멈춘 영상 프레임에서 Live Text 사용하기

멈춘 영상 프레임에서 라이브 텍스트 사용하기
(요부분 어렵스)
AVKit을 사용하면 멈춘 영상 프레임에서도 라이브 텍스트를 쓸 수 있다.

