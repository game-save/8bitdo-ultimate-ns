# 8bitdo-ultimate-ns

### [팔얼블 2.4 리시버로 스위치 모드 사용하기](https://gall.dcinside.com/mgallery/board/view?id=gamepad&no=18184)
```
<개요>
팔얼블이 많이 보급된 지금 알 갤럼들은 알다시피 팔얼블은 기본적으로 pc에 연결방식에 따라
2.4 리시버 -> 엑스박스 원
블루투스 -> 프로콘으로 인식된다.
(NS버전, 2022/12/07 기준)
다만 현재 동글 펌웨어를 베타버전으로 업데이트하면 2.4 리시버 -> 프로콘 인식이 가능하다

<순서>
1. https://web.archive.org/web/20230209193759/https://tempfiles.8bitdo.com/DODO/UltimateBLRR102B1m.zip에서 다운, 압축 해제
1.1 github에서 바로 받을 경우 : https://github.com/game-save/8bitdo-ultimate-ns/blob/main/UltimateBLRR102B1m.zip
2. PC에 리시버 연결, 팔얼블은 전원off (리시버-팔얼블 연결된 상태면 진행불가)
3. 8BitDo_UM_BT_Receiver 실행, USB Update 클릭, 같은 폴더 내 UM_BT_Receiver_V1.02_Beta1.dat 선택
4. 리시버 업데이트 완료 후, 팔얼블 켜서 리시버에 연결
5. SELECT(-버튼) + Y 5초간 눌러준다
여기에서 원래 설명에 따르면 팔얼블 LED가 깜박거리며 변경되었다고 나와야 하는데
일단 본인 팔얼블 기준으로는 그런 표시는 없었고
PC에서 기기가 연결, 해제되는 시스템소리가 몇번 난 뒤 팔얼블 전원이 꺼지고
이후 전원을 켜주면 자동으로 다시 페어링되면서 스위치 모드로 변경되어 있었음.

스위치 모드 말고도 다른 모드도 가능함
Switch mode: SELECT+Y (Apply for Steam Deck & Switch)
Xinput mode: SELECT+X (Apply for Windows 10 1903 or above)
Dinput mode: SELECT+B (Apply for Mister, Android and Linux)
Default mode: SELECT+START (Automatically identify Windows and Switch) <- 원상복귀

<자이로 설정(스팀)>
베타버전인지 아니면 팔얼블 특인지 스위치모드에서 자이로에 쏠림 있음. 이걸 스팀에서 잡아줄거임 (쏠림 없으면 안해도 됨)
reWASD도 비슷한 기능있다고 들었는데 스팀만 사용해봐서 스팀으로 올림

1. 왼쪽 상단 [Steam] - [설정] - [컨트롤러] - [일반 컨트롤러 구성]
2. 발견된 컨트롤러에서 [보정하기]
a04424ad2c06782ab47e5a67ee91766dc289f1edd1acc5cfbf10d2c159d2d3216cb3379582bbfde5ce884a3a744639
3. [자이로 전용 보정 시작] 클릭
4. 아래같은 창이 뜰건데 그냥 바닥에 내려두고 기다리면 알아서 보정해줄거야. 보정 끝나면 메세지 뜨니까 기다리셈
a04424ad2c06782ab47e5a67ee91766dc289f1edd1acc5cfbf10d2c158d1d42191a0d1011277ee0f12c786f115dc
5. 비스팀게임이면 스팀 라이브러리에서 왼쪽 하단 [게임 추가] - [비 Steam 게임 추가] 로 추가시켜서 실행하면 됨.

기타)
- 2.4g 스위치모드에선 스위치 프로파일 적용됨
```
