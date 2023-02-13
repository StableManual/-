# 합성 시작

## 합성을 위한 기능(Inpaint)
<br/>

![무제12_20230129183112](https://user-images.githubusercontent.com/123804566/215317664-4ec372b5-14f8-4766-8b2a-524895714f5a.png)

우리는 합성만 할것이니 Img2Img의
Inpaint 기능을 사용할거다.

> Inpaint 기능은 사진에 특정 부분만 AI가 처리하도록 시키는
기능이다. 잘 응용한다면 포토샵처럼 이용가능

![무제13_20230129183154](https://user-images.githubusercontent.com/123804566/215317667-f550de6f-18ca-4a85-a833-36b487227d6a.png)

![0129-174904_Crome](https://user-images.githubusercontent.com/123804566/215317748-2670de61-8ef5-404e-9158-c35e3d517520.jpg)

<br/>
<br/>

아래 설정들의 개념을 설명하자면 (합성때 주로 쓰는 설정은 굵은글씨)

***

**sampling steps : AI가 얼마나 사진을 검수할지 설정**

**CFG scale : 얼마나 프롬프트를 따를지 설정**

_just resize : 찌부려서 강제맞춤_

**Crop and resize : 남으면 잘라버림**

_Resize and fill : 가장자리만 늘려서 맞춤_

_just resize(Last Noize) : 마지막 생성단계 노이즈 잡아늘림_

_Fill : 원본 무시하고 새롭게 만듬_

**Original : 원본 참고해서 만듬**

**whole picure : 전체영역 생각하고 생성**

_Only masked : 따로 재생성 후 축소해서 박아넣음_

**padding pixels : 마스크 주변에서 몇 픽셀만큼 색,형태, 정보를 반영하는가**

**Denioising strength : 낮을수록 최대한 세밀한 영역만 수정 (원본에 가까움),
   높을수록 많은 부분 자유생성 (원본에서 동떨어짐)**

***

<br/>
<br/>
<br/>

## 합성시작

![무제14_20230129183654](https://user-images.githubusercontent.com/123804566/215317929-b83f8765-32e7-4540-9d7f-5103eb6e5e0b.png)
 
<br/>

자신이 인페인트할 사진을 불러온 후. 자신이 합성할 부분을 
칠해준다.

<br/>

![무제14_20230129183811](https://user-images.githubusercontent.com/123804566/215317930-2ed923c0-3d2d-4b77-a60b-6becfd956461.png)

그 후 프롬프트(긍정) 창에 Nude, Naked, (칠한 부분에 맞는 단어[가슴이면 chest 성기면 뭐뭐 등등 영어로..]) 입력

![2020129184448](https://user-images.githubusercontent.com/123804566/215318228-ba421f22-4ad3-4a7e-8821-eb72da2cec83.png)

약간 실망스럽게 나올거다. **포기하지마라 AI는 자신이 어떤 설정, 모델을 쓰고
인내심을 들이냐에 따라 다른 결과가 나온다..**
<br/>
그렇기에 설정을 약간씩 바꾸며 계속 생성해준다.
그리고 부자연스럽게 나온 부분의 특징을 프롬프트(부정)에 영어로 작성하면
더 좋은 결과를 얻을 수 있다.

![2030129184431](https://user-images.githubusercontent.com/123804566/215318323-35a1144b-61fc-4147-a1c8-71e432507be4.png)


난 이게 마음에 들었다

마음에 드는 사진이 나와도 피부 결계 자국이 나올 수 있는데 
이 경우에는 Send to Inpaint 버튼을 눌러주어 결과 사진을 다시 인페인트
할 수 있다. 
<br/>
<br/>
<br/>
<br/>

## 팁

* 다른 모델들

* 옷
   * 검은 옷
      * 검은 옷은 합성이 잘안되니 인페이트 스케치나 전작업
        이용하기
* 피부색 
   * 피부색 같게 하기
   * 피부가 어두워짐

* 신체
   * 손가락
      * 손가락에 관한 목록..
