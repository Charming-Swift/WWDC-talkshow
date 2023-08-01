# Meet SwiftData
> [video](https://developer.apple.com/videos/play/wwdc2023/10187)

## Talkshow
> 2023.07.31, 19:00 ~ 20:00 <br>
> 참여자: `다혜🐥`, `민규🍀`

<hr>

### 근황 토크
> WWDC 토크쇼가 7월동안 쉬었는데, 다들 어찌 지내셨는지요? (5분)

* `다혜🐥`: 안녕하세요! 오랜만입니다.
* `민규🍀`: 반갑습니다.
* `다혜🐥`: 이번 wwdc 토크쇼가 사실 7월 동안 좀 쉬었어요.민규 님도 꽤나 자주 방문해 주신 분 중 한 분이었는데, WWDC 토크쇼는 저와 봄이님이 주로 진행하는데 7월 동안 일정이 바빠서 공지도 못한 채로 쉬게 되었습니다..
* `민규🍀`: 그렇죠 괜찮습니다. 다들 바쁘지 않았을까요? 저도 KWDC 자원봉사자로 일하고, 다혜님도 KWDC 연사자로 준비하시느라 바쁘셨잖아요.
* `다혜🐥`: 그리고 휴가 갔다 오신 분도 있을 거구요. 잘 쉬었네요!!그동안 어떻게 지냈는지 간단하게 이야기를 들어보고 SwiftData에 대해서 얘기해 보죠.
* `민규🍀`: 저는 KWDC 자원봉사자를 신청해서 스태프로 잠깐 일하고 이제 취업 준비하고 이력서 쓰고 있습니다.
* `다혜🐥`: 이력서!
* `민규🍀`: 이력서를 노션으로 작성하다 보니 너무 비슷한 템플릿인 것 같아서 요즘에는 그냥 피그마로 작업하고 있습니다.
* `다혜🐥`: 오히려 그 독특함을 유지하기 위함인가요?!
* `민규🍀`: 마음대로 할 수 있으니까 무조건 좋은 것 같더라고.
* `다혜🐥`: 저도 노션은 그냥 1차 이력서로 쓰고 그거를 다른 형태로 옮겨서 작성하고 있습니다.지금 당장은 크게 구직 활동을 하고 있지는 않아요 ㅎㅎ;..
* `민규🍀`: 그렇죠 회사마다 또 이렇게 쓰는 것도 일이고 다른 거 할 것도 많이 쓰니까
* `다혜🐥`: 한 번은 아무것도 안 하고 좀 쉬고 싶긴 해요.지금 아니면 언제 쉴까 싶기도 하고.
* `민규🍀`: 다혜님 열심히 하셨잖아요.
* `다혜🐥`: 이번에 7월에 큰 행사인 KWDC 그걸 준비하느라 거의 모든 에너지를 쓴 것 같아요.
* `민규🍀`: 세션 준비하시면서 iOS 17이 엄청 기다려지셨을 것 같아요.
* `다혜🐥`: 맞아요 좋은 게 많더라고요. 얼른 얼른 적용됐으면 좋겠다라는 생각..
* `민규🍀`: 어느정도 근황을 들어본 것 같아요. 그러면 본격적으로 SwiftData에 대해서 이야기 해볼까요?

---

### SwiftData의 첫인상
> 이번에 나온 새로운 기술

* `다혜🐥`: SwiftData을 처음 봤을 때는, 어? 뭐지? 였어요. 예전에 이런게 있엇나? 했지만~근데 그게 아니라 완전히 처음 나온 거더라고요.
* `민규🍀`: 그렇죠.
* `다혜🐥`: 그래서 영상을 보면서 좀 깨달은 것도 있고 아직 어려운 점들도 있었는데, 일단 SwiftData에 대한 첫 인상을 각자 한번 얘기를 해볼까요?
* `민규🍀`: 영상 내용은 생략하고 첫인상은 CoreData이 생각났어요.CoreData를 약간 SwiftData로 다루나? 맞더라고요.
* `다혜🐥`: 처음부터 그렇게 생각을 하셨군요!!
* `민규🍀`: 약간 그걸 다루는 느낌 느낌으로, 네네.
* `다혜🐥`: SwiftData 소개할 때 이런 말이 있었거든요." 스위프트 ui와 마찬가지로 외부 파일 형식 없이 코드에만 집중한다 "뭘 코드에만 집중한다라고 왜 또 강조를 하는 걸까? 생각했는데 CoreData랑 비교하면서 얘기 하더라고요.CoreData가 테이블들을 코드로 작성하는 게 아니라 Xcode에서 따로 준비된 어떤 하나의 영역에서 끌어다 쓰는 거였잖아요.그래서 그 얘기를 하는 거구나." SwiftData는 그냥 Swift 코드로만 데이터 스키마를 작성할 수 있다 "이 얘기를 하고 싶었구나 알게되었죵.
* `민규🍀`: 그렇군요.
* `다혜🐥`: 그리고 SwiftData에서 사용하는 매크로도 생소한 개념었어요.
* `민규🍀`: 저두요.
* `다혜🐥`: 그래서 매크로랑 같이 복합적으로 얘기를 해서 처음에는 원리를 이해하기 어려웠어요.
* `민규🍀`: 저는 다혜님의 KWDC 세션을 듣고 봐서 그런가 매크로에 대한 개념이 어느정도 있어서 보는데 크게 어려움은 없었어요.
* `다혜🐥`: KWDC에서 제 세션을 들으시고 매크로에 대한 이해가 된 상태라서~!!
* `민규🍀`: 그렇죠 그래서 쉽게 느껴졌다.
* `다혜🐥`: 그러면 KWDC에서 SwiftData 세션이 따로 있었는데 그 세션은 혹시 들으셨나요?
* `민규🍀`: 제가 스태프 하고 있어서 다른 세션은 잘 듣지 못했어요.
* `다혜🐥`: 나중에 영상 나오면 한번 꼭 보세요.되게 좋았습니다. 토브 님이 해주신 세션인데 깔끔하고 좋았어요.
* `민규🍀`: 봐야겠어요.
* `다혜🐥`: 그리고 매크로와 관련한 세션도 있어서 그거 두 개 다 보시는 걸 좀 추천드립니다.
* `민규🍀`: 감사합니다. 네 8월 말에 올라온다죠?
* `다혜🐥`: 네네.
* `민규🍀`: 기다리기 힘듭니다. 제가 이미 다 봐버릴지도..
* `다혜🐥`: WWDC23 세션 먼저 보고 KWDC 세션을 보는 게 더 이해하기 좋을걸요?혼자서 먼저 소화를 한 다음에 2차적으로 이제 매실 음료수 마시는 거죠.달달하고 소화 잘 되는!
* `민규🍀`: ㅋㅋㅋ오오 그러면 먼저 들어야겠네요ㅎㅎ
* `민규🍀`: 그리고 SwiftData에서 이 약간 뭔가... SQL의 맛이 느껴진다랄까..쿼리가 나와서 그런가봐요.
* `다혜🐥`: 여기 나오죠 query!

(query 이미지)

* `민규🍀`: 그런 게 약간 좀 신기했다.
* `다혜🐥`: 저는 옛날에 Django를 다뤄본 적이 있는데, Django도 Python 언어로 데이터 스키마를 만들 수 있거든요.ORM이 생각나는 SwiftData였습니다. 그래서 저는 그 때 생각이 참 많이 났습니다.
* `민규🍀`: 오호
* `다혜🐥`: iOS에서도 Swift로 데이터 스키마를 정의할 수 있겠구나...추억은 방울방울 했습니다.
* `민규🍀`: 이해가 빨리 되셨겠네요.
* `다혜🐥`: 옛날에 과거의 경험을 도움을 좀 받았죠.그런데 이 뒷부분에 어려운 것들이 좀 있긴 했어요.이 컨테이너 개념 자체는 생소하더라고요.
* `민규🍀`: 저 컨테이너는 약간 직접 해보면 바로 이해될 것 같지 않아요?
* `다혜🐥`: 써보면?
* `민규🍀`: 네. 앱에 적용시켜 보거나 Xcode에서 써 보면은 개념도 쉽게 이해될 것 같아요.
* `다혜🐥`: KWDC에서도 컨테이너 설명을 좀 해주셨는데 100프로 이해한 건 아니었지만 WWDC 영상 혼자 볼 때보다는 훨씬 좋았습니다.나중에 올라오면 한 번 더 보려구요.
* `다혜🐥`: 그럼 첫 인상에 대한 얘기는 여기까지 해보도록 할게요.
* `민규🍀`: 네

---

### SwiftData와 CoreData
>둘의 차이와 CoreData 쓸 때의 느낌 + SwiftData 


* `다혜🐥`: 그래서 다음 질문!SwiftData를 쓰는 것에 대한 얘기도 좋은데 아무래도 이게 나온 배경에 CoreData가 있다고 보거든요.애플에서도 직접 설명했죠!SwiftData와 CoreData 이 두 개에 관해서 자유로운 얘기를 나눠보도록 할게요.
* `다혜🐥`: 둘의 차이와 CoreData를 썼을 때 경험, 그리고 그럼 여기에 SwiftData를 쓰면 어떤 문제점들이 극복될 것 같은지 자유롭게 이야기 해볼게요.
* `민규🍀`: CoreData를 직접 써보신 적은 있으신가요?
* `다혜🐥`: 저는 써본 적 있어요.
* `민규🍀`: 어디서 써보셨나요?
* `다혜🐥`: '가사오케'를 만들 때 썼었는데 그 프로젝트가 서버를 쓰는 건 아니거든요.정확히 말하면 노래방 노래 검색은 당연히 이제 외부 api를 쓰는데,노래방에서 부를 노래를 미리 보관하는 보관한 '노래 리스트'들은 기기에 저장이 돼요.그래서 그때 CoreData를 사용했습니다.
* `민규🍀`: 써본 느낌은 어떠세요?? 쓰기 편했나용?
* `다혜🐥`: 코어 데이터를 썼을 때 느낌은 그냥 써본 사람 다 알 거예요.이거 그냥 데이터베이스 테이블을 그대로 옮겨왔네.딱 이 느낌이에요.
* `다혜🐥`: 그리고 쓰는 방법도 사실 크게 어렵지는 않았어요.단지 CoreData로 데이터 스키마를 정의하려면 Swift 언어로 하는 게 아니에요. 외부적인 라이브러리를 쓴다는 느낌을 좀 많이 받았어요.정의하고 나면 Swift 코드로 정의된 데이터에 접근하는 건 됩니다.
* `민규🍀`: 저는 사실 CoreData를 써보지는 않았거든요.보기만 했다~그래서 자세히는 모르는데 저 인터베이스로 알고 있었어요.
* `다혜🐥`: 민규님도 전공자니까 DB를 배웠기 때문에 개념적으로는 어렵지 않으셨겠네요?
* `민규🍀`: 그렇져.너무 익숙한 것들이라서 네.
* `민규🍀`: CoreData와 SwiftData, 이거는 좀 생각해 보면 둘 다 동시에 쓸 수 있는 걸까요? 아니면 둘 중에 하나만 쓰는 걸까요?
* `다혜🐥`: 동시에 쓸 수 있지 않을까요? 개별적으로 사용할 수 있을 것 같던데.
* `민규🍀`: 그러면 SwiftData로 CoreData를 조작하고, 그 역도 가능할까요?
* `다혜🐥`: 아,
* `민규🍀`: 가능할까요?
* `다혜🐥`: 그건 안 되는 것 같아요. 그러니까 두 개가 다른 개념인데인거죠, 다르게 쓰이는 기술들인데
* `민규🍀`: 네
* `다혜🐥`: 단지 CoreData의 단점들을 SwiftData로 보완하는 관계인거요.저는 그렇게 이해를 했습니다.그래서 CoreData를 써 데이터를 SwiftData로 접근할 수 있느냐? 그거는 안 될 것 같아요. 여기까지 영상을 본 제 생각이었습니다.
* `민규🍀`: 페이지 내용에서 키과 관련된 내용도 했었던 것 같은데,클라우드 키이었나?
* `다혜🐥`: 클라우드 킷?
* `민규🍀`: 클라우드 킷이 코어 데이터를 관리하는 거죠.
* `다혜🐥`: 그런 가요? 저 클라우드 킷은 사용해본 적이 없어요.
* `민규🍀`: 여기 도큐먼트가 있는데, 이걸로 보아 하니 클라우드 킷으로 CoreData를 설정한 다음에 그 CoreData에 관해서 모델 컨테이너로 저장하고 그 모델 컨테이너를 뷰에다 적용시키는 거..인거죠.
* `다혜🐥`: 그러면 둘을 섞어서 쓸 수 있다는 말일까요?
* `민규🍀`: 뭔가 그런 것 같아요. 컨테이너를 갈아 끼워서 쓰잖아요.
* `다혜🐥`: 그럼 그 컨테이너로 공유를 하는 건가요? 데이터를?
* `민규🍀`: 이제 이 모델 컨테이너에 CoreData를 끼워넣는,, 이거 뇌피셜이긴 한데 다음 세션에 CoreData를 한다면 더 공부해서 설명을 드릴 수 있습니다.
* `다혜🐥`: 좋은데요. 약속하신 겁니다.
* `민규🍀`: 관련 세션으로 이 여러개 있더라구요.
* `다혜🐥`: 볼까요?다음 세션은, 놀랍게도 CoreData 세션입니다!!저희가 이제 세션 주제를 다 정해놓고 하는 하고 있어요.CoreData가 연결된게 많아서 이렇게 정해두고 있습니다.
* `민규🍀`: 아주 야무지게 해놓으셨네요. SwiftData 시리즈로.
* `다혜🐥`: 그렇죠 연속으로!
* `민규🍀`: 다음에 빌드도 해보고 코어 데이터도 한번 만들어보고 해서 한번 설명드릴게요.
* `다혜🐥`: 이 데이터로 간단한 메모장 앱을 한번 만들어봐도 재밌을 것 같네요.
* `민규🍀`: 클라우드 킷도 재밌겠는데요. 이러면 저희 백앤드가 필요 없는 건가요?
* `다혜🐥`: 글쎄요. 다른 플랫폼이랑 같이 쓰려면 외부 서버를 쓰는 게 좋을 것 같은데요?
* `민규🍀`: 아까 말씀하신 대로 메모장 같은 앱을 만들면서 배우면 좋을 것 같아요.
* `다혜🐥`: 좋습니다. CoreData를 안 써보셨다고 해서 직접적인 비교는 어려울 수 있지만 그래도 대충 어떤 느낌인지는 알고 계시니 이야기 하기 편했습니다.8월 동안은 SwiftData에 대한 얘기를 많이 할 것 같네요.

---

### 이해하기 어려운 점들, 같이 살펴봅시다.
>어려운 내용들 / 다음 세션에서 주의 깊게 보고 싶은 것들

* `다혜🐥`: 마지막 질문!중간중간 얘기가 나왔지만 SwiftData 세션을 들으면서 좀 이해하기 어려웠던 점들이나 이제 다음 세션에서 좀 주의 깊게 보고 싶은 것들 각자 얘기를 해보죠.
* `민규🍀`: 먼저 말씀드리면 모델 컨테이너는 좀 이해가는데 모델 컨텍스트는 약간 좀 어렵잖아요.
* `다혜🐥`: 아
* `민규🍀`: 그래서 모델 컨텍스트가 어떤 쿼리가 같은 것 같기는 한데, 다음 세션에서 한번 자세히 보려고 합니다.
* `다혜🐥`: 저도 컨테이너랑 콘텍스트 부분이 좀 생소했어요.마이그레이션을 지정할 수 있고 뭔가 하는데 모델 컨테이너에 정확한 사용 방법이나 그러니까 왜 쓰는지를 아직 이해를 못했습니다.그래서 다음 세션에서 이게 왜 쓰는지에 대해서 좀 집중 탐구를 해보려고 합니다.
* `다혜🐥`: 그리고 세션을 보는 것도 보는 건데 직접 코드를 쳐보는 과정이 필요할 것 같아요.
* `민규🍀`: 인정합니다. 네.
* `다혜🐥`: 그렇습니다.
* `민규🍀`: 마이그레이션 세션에 모델 컨테이너 내용이 나오나요?
* `다혜🐥`: 글쎄요 한번 봐야 알 것 같아요!
(중략)
네 좋습니다. 그럼 마무리해볼게요.이번 주는 (1)SwiftData 세션을 보고 (2)SwiftData란 무엇인가 그리고 (3)어떻게 쓰는가를 알아봤는데 이게 아무래도 새로운 개념이다 보니 낯선 건 맞는 것 같아요.헌데 낯설지만 그렇다고 아주 어려운 건 또 아닌 것 같습니다.
* `민규🍀`: 어렵죠
* `다혜🐥`: 다음 주에도 이 SwiftData와 관련된 세션들을 주제로 가지고 있으니 한번 이번 주에 몰랐던 내용들을 다음 주 세션 토크쇼 준비하면서 공부하시면 좋을 것 같아요.
* `민규🍀`: 감사합니다. 네
* `다혜🐥`: 다음 주는 "Build an app with SwiftData"입니다.마지막으로 하고 싶은 말씀 있으신가요?
* `민규🍀`: 너무 감사합니다.
* `다혜🐥`: 그러면 녹음 여기까지 하도록 할게요.
* `민규🍀`: 네.