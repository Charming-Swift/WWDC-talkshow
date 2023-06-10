# Go further with Complications in WidgetKit
> [video](https://developer.apple.com/videos/play/wwdc2022/10051/)

## Talkshow
> 2023.06.07, 20:00 ~ 20:50
> 참여자: `다혜🐥`, `민규🍀`, `대홍🎿`, `봄이💟`

<hr>

### (사담) WWDC 23 시작!

> 두근두근

* `다혜🐥`: 2023이 시작이 됐는데 영상 다들 한 번씩 보셨나요?
* `대홍🎿`: 저도 새벽 4시까지 봤습니다.
* `다혜🐥`: 저도 4시까지 봤거든요.
* `대홍🎿`: 네네.
* `다혜🐥`: 솔직히 좀 피곤할 것 같았어요. 왜냐하면 작년에도 WWDC를 생방송으로 봤었는데, 조금 피곤했던 기억이 나요.그래서 올해도 피곤하지만 참고 봐야지~ 했는데 이번에는 하나도 안 피곤하고 너무 재밌더라고요.
* `대홍🎿`: 생각보다!
* `봄이💟`: 저는 iPadOS까지 보고 잠들었습니당.
* `다혜🐥`: 아무래도 저희가 WWDC 토크쇼이니까 따끈따끈한 WWDC23에 대한 얘기를 조금 하고 본격적으로 진행하도록 하겠습니다.
* `대홍🎿`: 좋습니다.
* `다혜🐥`: 이번에 봤을 때 느낀 점은 "업데이트 사항이 진짜 많다!"였어요.저는 이번에 디스코드 커뮤니티에서 다른 분들이랑 같이 시청했어요.예전에 프로젝트 같이 하신 분들이랑 경력이 있으신 분들과 함께 봤는데, 그러다 보니 이것저것 여러 가지 이야기들을 들을 수 있어서 재밌게 보았습니다.행사 시작한지 2시간도 안되서 업데이트 사항이 엄청 쏟아져 나왔는데, 마지막에 VisionPro가 딱 나오면서 완전 절정이었죠.
* `대홍🎿`: 근데 저는 거기서 거의 잠이 와서ㅋㅋㅠㅠ 새로운 기기에 대해서 이야기는 들었는데 진짜 나왔더라구요.또 VisionPro가 좀 비중이 컸잖아요.
* `다혜🐥`: 많이 컸죠.
* `대홍🎿`: 초반에는 좀 놀랐다가 근데 이미 새벽 그때가 3시가 넘었더라구요?그때부터 이제 약간 몽롱해지면서 집중이 좀 흐려졌어요. ;-;
* `다혜🐥`: 같이 봤으면 재밌었을텐데, 아쉽다.
* `대홍🎿`: CharmingSwift 내부적으로 같이 봤어도 괜찮았을텐데. 당시에 따로 저희가 얘기를 한 게 없어서 못 모인게 아쉽네요.
* `다혜🐥`: 저희가 이벤트를 만들지 않았어서 그건 좀 아쉽긴 했어요.아무튼 저도 비전프로 처음 봤을 때 엄청 놀랬어요.애플이 AR 기기 만든다고 다들 알고 계시던데 근데 전 몰랐거든요.그래서 그때 공개할 때 알았고 놀람 다음에는 MS나온 홀로렌즈랑 비슷한 기기인가 보다 생각했어요.
* `봄이💟`: 홀로렌즈! 그것도 가격 비싸더라구요..
* `다혜🐥`: 제가 이거 연구실에 있는 홀로렌즈를 써봤거든요.내가 있는 공간에서 인터넷 창 띄우고 유튜브보고 게임하고 다 할 수 있었어요.그때 느꼈던건 선명함이 조금 떨어져서 어지러웠고, 생김새가 투박해서 어떻게 상용화가 잘 될까? 이런 생각을 많이 했었어요.
* `다혜🐥`: 근데 애플의 VisionPro는 기능도 일단 겉보기에는 다른 VR 기기가 가지고 있는 기랑 비슷한데 세련되게 만들었다.이 생각이 먼저 들었어요.
* `대홍🎿`: 같이 좀 놀란 게 네 애플 로고를 안 박아뒀더라고요.
* `다혜🐥`: 맞아요.
* `대홍🎿`: 보통 애플 얘네는 사과 마크를 항상 붙였는데 이번엔 웬일로 애플 마크를 뺐더라구요. 그래서 심미성에 집중했구나, 비싸겠다 싶었는데 역시나 비싸더라구요.
* `다혜🐥`: 크기는 크지만 스키 고글처럼 깔끔하게 만들었더라구요.시장에 나와봐야 알겠지마 개인적으로 가장 신기했던 건 그거였어요.비전 프로를 쓰고 사용자가 맥북을 켜니까 맥북에 있는 화면이 비전 프로로 옮겨가서 화면이 뜨는게 가장 신기했어요.
* `대홍🎿`: 그거랑 저는 또 놀란 게 사용하고 있다가 주변에 사람이 오면은 자동적으로 그 사람 쪽으로 화면이 살짝 흐릿해지면서 그 사람이 온 거를 알아차릴 수 있게끔 해주더라고요.
* `다혜🐥`: 맞아.
* `대홍🎿`: 그것도 좀 신기했어요.
* `다혜🐥`: 그냥 완전히 개발자를 갈아 넣었구나.어떻게 했지? 이 생각밖에 안 들긴 했어요.
* `대홍🎿`: 그 애 하나에 특허가 1500개인가까지 들어가 있대요.그거 보고 그럴 만하겠다 싶었어요.
* `민규🍀`: 저는 보면서 한가지 든 생각이, 시력에는 문제가 안될까였어요.
* `다혜🐥`: 다른 VR/AR 기기에서도 안경 쓰는 사람들이 그 도수 렌즈 같은 걸 맞출 수가 있다고 들었어요.
* `민규🍀`: 그것도 그런데, 티비를 가까이서 보면 눈이 나빠져서 근시가 오는 것처럼 눈 바로 앞에 화면이 펼쳐지니까 초고도근시가 되지 않을까 걱정되었어요.
* `대홍🎿`: 사람마다 시력 차이가 분명히 있을텐데 시력 보정이 들어가지 않을까요?
* `다혜🐥`: 가능할 것 같은데 지금 VisionPro에 있을지 모르겠네요. 1세대는 없어도 2세대는 들어가지 않을까요?시력 저하 문제, 이거 궁금하네요. 인터넷으로 검색해보겠습니다.

(인터넷으로 VR/AR 기기와 시력 저하의 관련성에 대해서 검색 중)

* `다혜🐥`: 따로 나오지는 않네요.
* `대홍🎿`: 제가 찾아보니까 내 눈앞에 아주 근거리로 비치는 영상이지만 저 멀리 저 깊숙한 곳에서 들어오는 빛이라서 공간감 조절이 되고 그래서 눈이 별로 필요하지 않다고 하네요.저희 창원에 가서 Charming Swift 발표 했었잖아요.
(Charming Swift 오거나이저인 대홍, 다혜, 민규, 봄이는 지난 5월 창원 USG 행사에서 커뮤니티 홍보와 관련하여 부스/발표를 한적이 있다)

* `다혜🐥`: 네.
* `대홍🎿`: 그때 행사에서 VR 기기를 체험할 수 있었는데, 사용했던 기기들이 다 어지럽더라고요.그래서 이 시력도 문제인데 약간 멀미 증상 오는 거를 또 어떻게 해결했을까? 궁금하기도 해요.
* `다혜🐥`: 영상에서도 멀미가 이유가 주변 시에 있는 레이아웃이의 선들이 흐릿해져서 초점을 못 잡아서 막 멀미가 난다고 하더라고요.그거를 잡아냈다고 했나? 기억이 잘 안 나네.
* `다혜🐥`: VisionPro 이야기를 먼저 했지만, 다양한 내용이 참 많았죠.앞서서 근시 이야기를 해서 그런데, iPadOS 업데이트 사항 중에 화면을 가까이서 볼 경우 너무 가깝다고 말해주는 어플을 만들었더라고요.
* `대홍🎿`: 그거랑 또 애플 watch에도 어린 자녀가 광합성을 얼마나 했는지 또 측정해 주는 그런 것도 있지 않았나요?
* `다혜🐥`: 맞아요.
* `대홍🎿`: 그러니까 이제 아기가 이제 애가 watch를 끼고 밖에 돌아다니면 이제 태양빛을 측정해서 몇 분 정도 했는지 알려주는 기능도 새롭게 업데이트가 됐더라고요.

<hr>

### Apple Watch 사용자를 찾습니다.

> 잘 쓰고 계시나요?

* `다혜🐥`: 새로운 업데이트 사항들이 기대되네요! 올 하반기에 iOS17이 나오면 얼른 업데이트 해봐야겠어요.그럼 본격적으로 이번 주 영상에 관련해서 이야기를 해보겠습니다.
* `대홍🎿`: 네!
* `다혜🐥`: 이번 영상의 내용은 WidgetKit에 관한 내용이었어요.애플 watch에 사용되는 Widget의 형태가 다양한데, watch를 쓰시는 분이라면 뭔 무슨 소리인지 알 거예요.
영상 내용 중에 시계 페이스에 따라서 같은 앱의 위젯이라도 형태가 다르게 나타난다. 이런 얘기들이 나오잖아요.라운드 처리된 위젯도 있고 그냥 한 줄짜리 위젯도 있고 그냥 뭐 동그라미로만 표현되는 위젯도 있고.다양한 Widget의 형태와 메서드에 대해서 이야기를 하고 있어요.그러면 두 번째 질문입니다. 혹시 애플 watch 쓰고 계신 분들 계십니까?
* `봄이💟`: 저요!
* `대홍🎿`: 저는 없습니다.
* `민규🍀`: 가지고 싶습니다.
* `다혜🐥`: 저도 현재 소유 중입니다.가지고 싶은 사람 두 명과 갖고 있는 사람 두 명이네요.
* `다혜🐥`: 그렇다면 애플 watch를 가지고 계신 분들! 주로 watch를 어떻게 활용하고 계신가요?봄이님부터 말씀해 주시면 감사하겠습니다.
* `봄이💟`: 저는 시계 기능으로 많이 써요.그거 말고는 날씨랑 가끔씩 네이버 페이 아니면 카카오페이를 사용합니다. 노래도 많이 들어요.
* `다혜🐥`: watch로 노래를 틀고 듣는 건가요?
* `봄이💟`: 아니죠. 에어팟이 연결되어 있죠.
* `다혜🐥`: 정리하면 아이폰에서 노래를 듣는데 그거를 watch로 조절한다는 거네요.
* `봄이💟`: watch에 유튜브 뮤직 앱이 깔리거든요. 아니면 그냥 애플 뮤직을 쓰거나. 멜론은 잘 모르겠어요.아무튼, 휴대폰에서 틀어놓으면 '지금 재생 중'이라고 뜨면서 휴대폰으로 watch로 조절할 수 있어요.
* `다혜🐥`: 저는 운동할 때 아주 잘 쓰고 있습니다. 주로 나이키 러닝 앱(NRC)을 씁니다.watch가 없을 때는 허리에 휴대폰을 차고 앱을 켠 다음 달리기를 했어요.NRC는 제가 달린 거리와 페이스 이런 게 기록해줘요. 근데 뛰는 도중에는 제가 몇 킬로 남았는지를 알기 힘들었어요.휴대폰을 허리에 차고 있으면 그 뛰는 동안 못 본단 말이죠.근데 watch가 있으니까 그냥 손목에서 확인이 가능하고 바로 체크가 가능한게 좋았어요.
* `다혜🐥`: 두 번째로는 아무래도 심박수가 기록이 된다는 점...저의 운동 능력이 데이터화 되는 것 같아서 좋더라고요.운동 말고 쓰는 거는 watch로 알람이 오니까 휴대폰을 손에 안 잡고 다닌다? 그 정도 입니다.
* `대홍🎿`: 혹시 watch에 전화도 오나요?
* `다혜🐥`: 전화 와요. 저는 운동 중에 전화 오면 그 watch로 받아요. 뛰면서 전화합니다 ㅋㅋ
* `대홍🎿`: 문자도 되는 거예요?
* `다혜🐥`: 문자도 간단하게 답장을 할 수 있어요.
* `대홍🎿`: 그러면은 제가 휴대폰을 예를 들어서 안 들고 러닝을 뛰고 싶으면 집에 휴대폰 놔두고 뛰어도 되나요?
* `봄이💟`: 그건 셀룰러 모델만 가능해요.
* `다혜🐥`: 셀룰러가 아니면 두 기기가 블루투스로 통신을 하기 때문에 watch가 휴대폰이 가까이 있어야 사용이 가능해요.저는 뛸 때 휴대폰은 그냥 허리춤에 차고 있고 watch로 모든 걸 다 해요.
* `민규🍀`: 셀룰러는 요금도 더 내야해요. 개통을 따로 해줘야 하는 걸로 알아요.
* `다혜🐥`: 이렇게 애플 watch 쓰는 거 들어보니까 어때요? 사고 싶나요?
* `대홍🎿`: 저는 지금도 마켓을 매일 뒤져보고 있거든요.특성상 전자제품은 또 무조건 새 걸 사야 되는 사람의 욕심이 있어서...근데 너무 비싸서 고민됩니다. 시계 하나에 운동할 때 잠깐 쓰고 시계 잠깐 쓰기만 할 것 같아서요.
* `다혜🐥`: 여건만 되면 바로 구입하시겠는데요.
* `대홍🎿`: 근데 진짜 별 생각 없다가 요즘 운동하면서부터 너무 필요하다느 생각을 많이 해요.또 주변 사람들이 다 운동하는 사람들 얘기를 들어보니까 진짜 휴대폰처럼 쓰고 계시네요.아까 보미 님이 말씀하신 것처럼 노래도 바꿀 수 있고 하는 걸 들어보니까 큰일 났네요.
* `다혜🐥`: 오늘을 기점으로 또 변화가 있겠네요.
* `대홍🎿`: 가격이 조금만 낮으면 괜찮은데 솔직히 더 찾아보면 살 것 같아서 안 찾아봤어요.
* `다혜🐥`: 저도 사실 저도 이걸 선물받아서 제가 잘 쓰고 있어요.너무 사고 싶어서 가격 알아보면 다시 살 마음이 사라지고 그랬습니다...
* `대홍🎿`: watch도 그러면 저희 그냥 일반 아이폰처럼 배터리 효율 이런 게 있나요?
* `다혜🐥`: 네 있어요!그리고 watch로 유용하게 쓰고 있는 기능이 알람이에요.제가 소리를 듣고 잘 못 일어나요. 그래서 watch 차고 있으면 알람을 진동으로 알려주거든요.제 삶에 일부가 되어버렸습니다..


<hr>

### WidgetKit, 영상을 보고 나서 생각들

> 연관된 영상이 많더라구요 ^^;

* `다혜🐥`: 그러면 세 번째 질문 가보겠습니다. .그래서 영상을 보고 나서 어떤 생각이 들었는지를 좀 얘기를 해보려고 하는데요.
* `대홍🎿`: watchOS는 어떻게 개발이 되고 적용되는지 궁금했어요. 그래서 영상을 쭉 시청했는데, 크게 와닿는 느낌은 없었던 것 같아요.아무래도 watchOS를 이용해서 개발을 해본 적도 없어서 그런 것 같기도 해요.그리고 마지막 부분에 마이그레이션 부분이 좀 어려웠어요.
* `대홍🎿`: 이 영상 초반에 잠깐 언급됐던 부분이 이 영상을 보기 전에 다른 영상을 더 보고 참고 영상을 보고 오면 조금 더 이해가 잘 될 수도 있다라고 얘기를 했는데, 제가 그 영상을 안 봤거든요. 그래서 이해가 더 어렵지 않았나 싶습니다.그래도 다음에 기회가 된다면 한번 watchOS가 이번에 또 업데이트가 되어서 더 학습해보고 싶은 생각이 들었습니다!
* `다혜🐥`: 저도 공감하는 부분이 있는 게 여기 영상 초반에 보면 이렇게 이거 듣고 오라고 하거든요.그래서 이 영상 하나로는 확실히 이해하기 어렵겠다 라고 생각하면서 시청을 했어요.이번 영상은 제가 watch를 쓰면서 사용을 했던 그 위젯들, 그 경험을 중심으로 영상을 이해를 하려고 했고요.개발적인 내용이 사실 이게 나오긴 했어도 그냥 그렇구나 정도로만 넘어갔어요.그리고 마지막에 마이그레이션 한 부분은 아마 이 클라킷이라는 게 옛날에 쓰던 거고 이거를 이제 새로 나온 위젯 킷으로 마이그레이션 하는 걸 알려주는 거로 저는 이해를 했어요.그래서 나중에 관련 영상을 보고 이번 영상을 다시 보는 게 좋겠다라는 게 저의 결론이었습니다.
* `다혜🐥`: 아무래도 저희들이 영상을 선택할 때 그냥 제목만 보고 선택을 했어서 이런 선수 영상들을 파악을 하기 어렵지 않았나 싶거든요.그래도 watch와 위젯 킷에 대해 생각할 수 있어서 좋았어요.
* `대홍🎿`: 전반적으로 재밌게 봤습니다!

<hr>

### WatchOS 개발

> 해보셨거나, 관심있거나, 계획 중에 있거나!

* `다혜🐥`: 그러면 다음으로 넘어가 보겠습니다. WiddgetKit에서 뭔가 얘기를 하기에는 어려울 것 같고, WatchOS 개발과 관련해서 말씀드려볼게요.그러면 오늘 참여하신 분들에게 WatchOS 개발에 관심이 있는지 궁금합니다!
* `민규🍀`: 옛날 삐삐 감성 앱을 watch 앱으로 만들어보고 싶어요.사용자 한명 당 아이디를 부여해서 8자리의 글만 보낼 수 있어요. 메신저처럼 삐삐 내용을 보낼 수 있는 거죠.
* `다혜🐥`: 와우 숫자만 보낼 수 있나요?
* `민규🍀`: 넵 그렇습니다. 그게 감성 포인트에요.
* `대홍🎿`: 저는 여행 다닐 때 사용할 watch 전용 번역 앱이 있으면 좋을 것 같아요. 기본 앱으로 있는지는 잘 모르겠지만...watch에 녹음 기능도 있다 했으니까 그 사람의 말을 받아서 이제 번역을 해주는 거죠.휴대폰으로 번역하면 디스플레이가 커서 보기는 더 편한데 급할 때는 watch로 해버리는 겁니다!
* `다혜🐥`: 있는지 없는지 확인해볼까요?

(확인중)

* `다혜🐥`: 일단 2022년 5월 기준으로, 파파고와 구글 번역, 네이버 사전 모두 watch용 앱이 없네요.
* `대홍🎿`: 오호.
* `다혜🐥`: "빠르게 번역한다"에 초점을 맞춰서 번역한 내용을 음성으로 알려주면 편할 것 같네요.
* `대홍🎿`: 그걸 노리는 거죠.
* `다혜🐥`: 좋아요. 좋아요. 일단 봄이님도 관심이 있으신가요?
* `봄이💟`: 저는 새로운 아이디어가 있는 건 아니고 저희 학교 과 친구들이 기숙사 식단 앱인 "아랑별"을 만들었는데요.그 앱을 watch에도 사용할 수 있게 하면 너무 편할 것 같아요.제가 만들어도 되냐고 물어보고 싶은데 아직 학기 중이라 아직 진행된 사항은 없어요.
* `다혜🐥`: 학교 다닐 때 급식표 찢어서 카드 카드처럼 들고 다니는 친구들 있잖아요.
* `봄이💟`: 있었죠 맞죠
* `다혜🐥`: 그 친구들이 만들었던 금식표 사이즈가 watch 사이즈와 비슷한 것 같은데, 좋은 아이디어 같습니다.
* `봄이💟`: "아람별" 앱이 제 맥북에도 설치되어 있어서 맥북 위젯에도 추가가 가능해요.그래서 저는 휴대폰이랑 맥북에도 모두 설치했는데, 이제 그것도 이제 귀찮아서 그냥 watch로 보고 싶을 때가 있단 말이죠.그래가지고
* `다혜🐥`: 저도 옛날에 watch 없을 때 생각한 아이디어가 있어요.아침에 대중교통을 타면 너무 피곤해서 졸았던 적이 엄청 많거든요.여기에서 내려야하는데 존다고 한 정거장 늦게 내리는 경우가 종종 있었어요.그래서 내가 내려야 하는 지점이 다와가거나, 한 정거장 전인 경우에 알림을 주는 앱이 있었으면 좋겠다고 생각했어요.이거 완전 대박 아이디어다! 했는데 이미 카카오맵에서 제공하더라구요.
* `봄이💟`: 아이고,,
* `다혜🐥`: 진짜 이 생각을 하고 미쳤다. 내가 회사 하나 차려야겠다 했는데 그래서 이제 이미 있다는 사실을 알고 내 세상이 무너졌어요.
* `대홍🎿`: ㅜㅜ아쉽습니다..


<hr>

### Watch와 Widget


* `다혜🐥`: 그러면 술 마무리로 가볼게요. watch와 widget에 대한 게 오늘의 마지막 질문입니다.근데 이미 앞에서 많이들 말씀을 해 주셔서 자유롭게 관련한 생각을 공유해주시면 감사하겠습니다.
* `다혜🐥`: 저 watch 쓰면서 watch 안에도 그 앱을 모아보는 게 있어요. watch에서 우측 크라운 버튼을 누르면 나의 watch 앱들을 모두 볼 수 있어요.근데 앱 서랍까지 들어가서 앱을 찾아 누르는 것보다 그냥 watch 페이스에서 위젯 설정한 걸로 들어가는 게 훨씬 훨씬 많단 말이죠.
* `봄이💟`: 공감합니다.
* `다혜🐥`: 맞죠. 그래서 이 widget이라는 게 watchOS를 watch 앱을 개발하려면 정말 필수적이다.그래서 watch와 widget은 꼭 같이 가져가야 되는 거라고 생각을 합니다.아이폰에서는 위젯 꼭 할 필요는 없지만 watch는 꼭 해야한다.. 이런거죠.
* `봄이💟`: 그렇죠.

<hr>

### 마무리

* 다혜🐥: 애플 watch에서는 필수다. 필수. 네 좋습니다.그러면 오늘 마무리를 해볼게요. 마지막으로 오늘 주제 관련해서 하고 싶은 말이 있으실까요?
* `대홍🎿`: 애플 워치 사고 싶다.
* `봄이💟`: 저는 사는 걸 정말 추천드려요.
* `대홍🎿`: 애플 워치가 SE가 있고 숫자 시리즈가 있더라구요. 차이가 있나요?
* `봄이💟`: 숫자 시리즈들을 사는 의미는 딱히 없는 것 같아요.누가 선물해주면 모르겠는데 내 돈 주고 사는데 굳이 그 정도까지의 스펙은 필요 없다고 생각해요.그래서 SE도 충분하다고 생각합니다.저는 오히려 숫자 시리즈가 오버 스펙이에요. 알림 잘 오고 시계 잘 보이고 하면 되는거라 딱히 숫자 시리즈 안사셔도 됩니다.
* `다혜🐥`: 마무리는 애플 watch가 구입하고 싶다로 끝이 났네요.
* `대홍🎿`: 영상에 대한 원래 그런가요? 영상에 대한 이야기보다 다른 부가적인 이야기가 더 많은 것 같아.
* `봄이💟`: 네 저희 토크쇼잖아요.
* `다혜🐥`: 원래 이거 영상에 관련해서도 얘기 많이 하는데 이번 주제는 더 그랬네요. 기술적인 이야기도 많이 합니다.예전에 ScreenTimeAPI 할 때는 얘기 많이 했어요.
* `다혜🐥`: 일단은 오늘은 여기까지 하고 다음 주는 2023 영상으로 한번 만나뵐게요.저희가 영상 리스트는 아직 안 뽑았지만 혹시 여건이 되신다면 2023 영상에서 추천을 좀 받겠습니다.일단은 다음 주 영상은 뭐가 될지는 제가 공지로 알려드리도록 할게요.이번 주도 재밌었고 즐거운 한 주 되시길 바랍니다.
* `봄이💟`: 수고하셨습니다. 다음에 뵐게요!
* `다혜🐥`: 그럼 오늘 여기까지 할게요~수고하셨습니다.