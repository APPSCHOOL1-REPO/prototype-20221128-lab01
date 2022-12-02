# Cherry(체리)

## 앱 정의(ADS)
블록체인과 연동하여 NFT의 메타데이터를 이용, 명함을 커스터마이즈 하고 공유할 수 있는 어플입니다.

## 주요기능
다중명함 생성 지원(최대 10장)

- NFT는 하나만 갖고 있는 경우는 드뭅니다. NFT에는 여러 프로젝트가 있고 각각 프로젝트에는 고유의 커뮤니티가 있습니다. 특정 커뮤니티에 나를 소개할 때는 그 프로젝트가 속한 NFT로 명함을 만드는게 아무래도 서로를 알아보기에는 더 쉬울 것입니다. 이런 분들을 위해 Cherry에서는 다중 명함 제작을 지원합니다.

소셜 서비스 연결

- NFT 커뮤니티 활동은 대부분 Web2.0 플랫폼 위에서 이루어집니다.
인스타그램, 유튜브채널, 페이스북 등 내 소셜 계정들을 명함에 포함할 수 있습니다
클릭 한번에 접근할 수 있게 자동으로 링크도 연결되니까 주변에 알리기도 간편합니다.

다른 사람 명함 추가, 보관

- 명함 고유의 URL이나, 아니면 만나서 QR코드를 찍어서 
다른 사람에게 받은 명함은 스토리지에 보관할 수 있어요.

명함 커스텀 기능

- 명함의 앞면과 뒷면을 각각 원하는 템플릿을 선택할 수 있습니다.
현재는 베타 버전이여서 특정 템플릿만 할 수 있지만, 확장되면 자유로운 템플릿에서 사용할 수 있게 할 계획입니다.


## 활용한 기술
- SwiftUI
- Glaip
- Moralis

## 원래 무엇을 목표로 한 앱이었는가?
- NFT의 메타데이터를 이용한 명함을 만들 수 있는 기능을 제공하고, 명함을 쉽게 저장/내보내는 기능을 제공하는 서비스

## 어떤 피드백을 받아 어떻게 개선했나?
피드백  

- 명함의 크기가 작습니다.
  
개선방안  

- 명함 크기를 키우고, 카드에 쉐딩을 주어
  더 명확하게 볼 수 있게 수정하였습니다.  
  
<img width="209" src="https://user-images.githubusercontent.com/98198645/205234453-1fdaaddf-0f26-4542-9e25-594d1d3d9303.png"> <img width="209" src="https://cdn.discordapp.com/attachments/1043032747112923166/1048130140019884052/ezgif.com-gif-maker_.gif">  

* * *

피드백  

- 컨텍스트 메뉴가 LongPress 방식이라 
  직관적으로 알기 어렵고, 기능 작동이 불편
  
개선방안  

- 컨텍스트 메뉴를 좀더 직관적으로 알아볼 수
  있게 변경하고, 터치 방식으로 기능을 변경
  하였습니다.
  
<img width="209" src="https://user-images.githubusercontent.com/98198645/205235546-836c2b0c-872e-4aa3-9144-a92fa77f22d1.png"> <img width="209" src="https://cdn.discordapp.com/attachments/1043032747112923166/1048130140586123264/ezgif.com-gif-maker_2.gif">  

* * *

피드백  

- 앱의 컬러가 통일이 안되어 있다.

개선방안  

- 전반적으로 모든 뷰에 메인컬러를 적절하게
  넣어 통일성을 부여함.

  
<img width="200" src="https://user-images.githubusercontent.com/98198645/205235753-4da2ca78-56c3-408c-ad5d-deead1d823b7.png"> <img width="209" src="https://cdn.discordapp.com/attachments/1043032747112923166/1048134379035164672/ezgif.com-gif-maker.gif">  
 
 * * *

피드백  

- QR 탭바의 아이콘이 어떤 기능을 하는지
  직관적으로 알기 어려웠다.
  
개선방안  

- QR 탭바의 아이콘을 변경, 그리고 텍스트를
  추가하여 탭바의 기능을 사용자가 직관적으로
  이해할 수 있게 수정하였습니다.
  
  
<img width="200" src="https://user-images.githubusercontent.com/98198645/205236638-681839c5-dfd3-4d2e-94f6-497754cbc92e.png"> <img width="200" src="https://user-images.githubusercontent.com/98198645/205236464-9f26ec72-c174-4e33-9d5f-ab2acf8aacc0.png">  

* * *

피드백  

- 명함보관함이 그룹보다는 다른 방식으로
  보여주는게 좋을 것 같다.

  
개선방안  

- 그룹안에 명함이 리스트 방식으로 보이도록
  개선하였습니다.

  
  
<img width="197" src="https://user-images.githubusercontent.com/98198645/205236360-41ca1b22-87bc-4e93-9e0a-d89ded57c271.png"> <img width="200" src="https://cdn.discordapp.com/attachments/1043032747112923166/1048130139587883008/ezgif.com-gif-maker.gif"> 



## 실제 MVP 구현을 위해 예상되는 도전과제 및 고민거리
로그인 세션 유지
- 현재 메타마스크 로그인 기능.  
하지만 세션을 유지하는 구현을 한번도 해 본 적이 없음.  
파이어베이스의 적절한 기능을 통해 할 수 있을 것으로 예상됨.

명함 꾸미기 기능
- 명함을 원하는대로 꾸미는 기능이 정말 어려울 것으로 예상됨.  
만약 노션처럼 엄청난 자유도로 꾸밀 수 있는 기능을 제공하려면, 그 자체가 워낙 난이도가 높아서 사실상 불가 할 것으로 생각됨.  
따라서 정해진 템플릿으로만 선택할 수 있게 하는 기능을 생각중

명함 공유
- 가장 고민이 많았던 부분. 
하지만 명함의 정보를 json 형태로 정리해서 QR코드에 담고,  
상대방이 QR코드를 찍으면 딥링크를 통해서 어플이 열리고,  
받아온 정보를 해당되는 명함의 템플릿에 널어주기만 하면 구현은 가능 할 것으로 예상됨.

## 참여자

| <img src="https://avatars.githubusercontent.com/u/33450365?v=4" width=200> | <img src="https://avatars.githubusercontent.com/u/104570633?v=4" width=200> | <img src="https://avatars.githubusercontent.com/u/98198645?v=4" width=200> | <img src="https://avatars.githubusercontent.com/u/98254580?v=4" width=200> | <img src="https://avatars.githubusercontent.com/u/86897750?v=4" width=200> |
| :----------------------------------------------------------: | :---------------------------------------------: | :-------------------------------------------------: | :-------------------------------------------------: |  :-------------------------------------------------: |
| 은노<br/>[@Eunno-An](https://github.com/Eunno-An)<br/> | 성민1<br/>[@mrgroomy](https://github.com/mrgroomy)<br/> | 혜성<br/> [@angry-dev](https://github.com/angry-dev)<br/> | 종환<br/>[@JJH0729](https://github.com/JJH0729)<br/> | 근섭<br/>[@JKSeub](https://github.com/JKSeub)<br/> |
