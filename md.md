#1. 문제 정의

##1.1 필요성    

최근 노크귀순, 지뢰도발 사건 등 북한의 군사적 위협 빈도가 나날이 증가하고 있다.
그에 반해 DMZ에 설치된 감시체계는 적의 움직임을 제대로 탐지하지 못하는 경우가 속출 하고 있다. 지난 지뢰도발사건 때 북한의 목함지뢰 매설 장면을 군이 보유한 CCTV로 파악하는데 실패하였다. 이 사건이후 열린 고위급회담에서 북한이 매설했다는 심증 이외의 물증을 확보하지 못함에 따라 북한의 지뢰도발을 정확하게 입증하지 못했다. 또한 귀순 사건시에도 북한군의 움직임을 포착하지 못해 귀순 희망자가 직접 노크를 해서 귀순의도를 밝히는 굴욕적인 장면도 있었다. 이와 같은 사건이 지속되면 북한의 도발 및 남침에 대한 조기경보를 할 수 없기 때문에 큰 전력의 공백이 예상된다.
CCTV는 기본적으로 Pan, Tilt, Zoom의 세 가지의 움직임을 제공한다. 하지만 이는 CCTV가 고정되어있는 정적인 상태에서의 움직임으로서 사각지대의 발생을 야기한다. 또한 사람에 의해 조작 및 감시가 수행됨으로 체력, 집중력과 같은 인체의 한계에 의해 감시 효율이 떨어진다. 사각지대의 발생을 해결하기 위해서는 정적인 CCTV를 만드는 요인인 인적자원, 전원, 데이터 전송, 조작문제를 해결한 동적인 CCTV 시스템이 요구된다.  

![image1](http://postfiles15.naver.net/20151211_126/hdhpow_1449813058917dvC96_PNG/PIC2079919174.png?type=w1)  

![image2](http://blogfiles.naver.net/20151211_17/hdhpow_1449813059392CVTqU_PNG/PIC2079919178.png)

![image3](http://blogfiles.naver.net/20151211_300/hdhpow_1449813059181Ix7QX_PNG/PIC2079919176.png)

<br>
<br>

##1.2 문제정의

**문제 정의**    
최초로 인식되어진 문제는 다음의 두 가지로 정의 된다.

1. 병사들의 시각 및 TOD를 이용한 감시는 체력, 집중력 등 인체의 한계가 있음.
2. CCTV의 dead zone발생


이 문제들의 본질적인 문제를 확인하기 위해 5Whys 방법을 사용한 결과는 다음과 같다.

####1.2.1. 병사들의 시각 및 TOD를 이용한 감시는 체력, 집중력 등 인체의 한계가 있음.
Why1. 왜 체력, 집중력의 한계가 있는가?  
Ans1. GOP 병사들의 인원이 적고 선진병영문화의 부작용으로 나태함이 생김.

Why2. 왜 GOP 병사들의 인원이 적고 선진병영문화를 시행하였는가?  
Ans2. 현역 복무 인원이 감소함에 따라 GOP에 할당되는 TO가 감소되었다.
     또한 복무 부적응자가 증가함에 따른 선진병영문화가 실시되었다.

Why3. 왜 현역 복무 인원이 감소하였고 복무 부적응자가 증가하였는가?    
Ans3. 출산률이 감소함에 따라 복무적합 병사가 줄어들었고, 복무적합 병사를 늘리기 위해 기존에 비해 현역 복무적합 기준을 완화시켰기 때문에 부적응자가 증가.

**이 문제를 해결하기 위해서는 사회의 전반적인 시스템 개선이 요구됨으로 해결이 어려움.**

####1.2.2. CCTV의 dead zone발생

Why1. 왜 GOP의 CCTV는 dead zone이 발생하는가?  
Ans1. 현재 설치된 CCTV는 고정된 상태에서 회전하는 정적인 움직임 밖에 되지 않는다.

Why2. 왜 정적인 움직임 밖에 지원하지 않는가?  
Ans2. CCTV 전원, 데이터 전송의 문제가 있고 조작은 병사가 수동으로 진행하기 때문이다.
	
Why3. 전원, 데이터 전송, 조작문제는 왜 발생하는가  
Ans3. CCTV는 신뢰성 높은 움직임을 보여야 하기 때문에 전원과 데이터 전송 시스템을 
     고정형으로 설치하는 경우가 많고 한사람이 다수의 CCTV를 조작해야하기 때문에 
     동적인 움직임의 CCTV 운용이 어렵다.

**문제**

>CCTV의 정적인 움직임을 탈피하기 위해서 인적자원, 전원, 데이터 전송, 조작문제를 해결한 동적인 CCTV 시스템을 통해 CCTV의 dead zone 문제를 해결해야 한다.

##1.3 요구사항

문제에 대한 요구사항은 다음과 같다. 

>1. 동적인 움직임을 할 수 있는 CCTV여야 한다.

>2. 운용병사의 수동조작이 필요 없어야한다.

>3. 스스로 적의 움직임을 인식할 수 있어야한다.

>4. 상시전원 및 보조전원을 이용하여 신뢰성 높은 전원공급이 이루어져야 한다.

>5. 네트워크를 통해 실시간으로 영상 및 이상을 보고 한다.

>6. 네트워크 상태가 좋지 않은 경우 delay-tolerant한 영상전송을 한다.
   긴급 상황 발생 시 주변 CCTV와 근거리 네트워크로 통신하여 네트워크가 정상인 
   CCTV가 상황을 보고한다.

>7. 야간에도 감시가 가능해야한다.

<br>
<br>

#2. 해결 방안 및 유사 사례
##2.1 기존 유사 제품
우리의 아이디어와 유사한 상용제품이 있는지 검색해보았다. 검색 결과 프랑스의 TEB이라는 CCTV 전문회사의 TUB라는 CCTV 솔루션이 우리의 아이디어와 유사한 점이 있었다. 

![image4](http://postfiles4.naver.net/20151211_67/hdhpow_1449813059854863BG_PNG/PIC2079919198.png?type=w1)
**그림1. TAB사의 TUB 제품 개요**

이들 또한 기존의 PTZ 카메라의 정적인 움직임을 해결하고자 하였고 이를 레일 시스템을 통해 해결했다. 레일 시스템 상에 PTZ카메라가 자유롭게 움직이게 함으로서 사각지대를 없앴다. 또한 이 시스템을 통해 우리가 실현하고자 했던 예산 절감이라는 목표를 달성하고 있었다. 

##2.2 기존 제품과의 차이점

  우리의 아이디어는 기존의 TUB제품과 비교하여 다음 표1과 같은 차이점을 가지고 있다.


![image5](http://postfiles9.naver.net/20151211_152/hdhpow_1449813060432gjRCF_PNG/PIC2079919212.png?type=w1)
**표1. TUB와 우리의 아이디어의 차이점**

  TUB는 제한적인 규모에서의 활용을 목적으로 개발되어 있다. 따라서 CCTV노드 상호간의 통신을 지원하지 않는다. 또한 동작의 신뢰성이 전반적으로 설치된 장소의 기반시설에 의존한다. 따라서 기반시설에 문제가 생기면 감시 시스템도 같이 문제가 생긴다. 

<br>

##2.3 우리 아이디어의 장점
우리의 아이디어는 야간 감시가 가능하다. 우리가 고안한 시스템은 적외선 LED를 탑재한 PTZ 카메라이다. 따라서 야간에도 제한된 거리 내에서 지속적으로 감시를 지속할 수 있다. (야간 탐지 가능 거리는 LED의 조도와 개수에 따라 달라진다.) 또한 TUB와 다르게 스스로 움직이는 물체를 탐지하고 보고한다. 이를 통해 사람에게 완전히 의존하지 않는 시스템을 제공할 수 있다. 우리의 아이디어는 하나의 레일에 여러 대의 CCTV의 연결을 지원한다. 이를 통해 기존의 TUB가 가지고 있던 다른 공간으로 이동시의 dead zone 발생을 해결 할 수 있다. (물론 기존의 고정식 CCTV를 설치하는 것에 비해 적은 대수로 움직인다.) 
TUB는 전원과 네트워크에 대한 보조적인 장비가 지원되지 않는다. 따라서 네트워크나 전원의 단선 시 시스템이 동작불능 상태에 빠진다. 반면에 우리의 시스템은 일정한도 안에서 네트워크나 전원의 문제가 있더라도 신뢰성을 유지하며 지속적인 감시가 가능하도록 설계 되어 있다. (여기에서의 일정한도는 배터리의 용량 사용하는 네트워크 시스템에 따라 상이하다.) 

##2.4 문제 해결을 위한 아이디어
####2.4.1 idea 1

![image6](http://postfiles12.naver.net/20151211_187/hdhpow_1449813060745GqSmq_PNG/PIC2079919220.png?type=w1)
>동적인 움직임을 위한 Rail System 채용   
>레일 위를 움직이게 함으로 사각지대를 예방

####2.4.2 idea 2
![image7](http://postfiles10.naver.net/20151211_105/hdhpow_1449813063186P3rc1_PNG/PIC2079919224.png?type=w1)
>기존의 정적인 PTZ CCTV의 제한된 탐지 범위를 확대가능

####2.4.3 idea 3
![image8](http://blogfiles.naver.net/20151211_63/hdhpow_1449813063651LyuwT_PNG/PIC2079919228.png)
>차영상을 이용하여 움직이는 물체 탐지 및 추적   
>스스로 적의 움직임을 탐색 및 운용병사의 수동조작 감소   
>IR 카메라를 통해 야간 감시 가능

####2.4.4 idea 4
![image9](http://blogfiles.naver.net/20151211_65/hdhpow_1449813063899RVtJu_PNG/PIC2079919232.png)
>**LTE 등의 일반 통신망 마비 시**   
>이상상황 미 발생 시 : Delay-Tolerant Network   
>이상상황 발생 시 : Wireless Sensor Network를 통한 이상상황 보고

<br>
<br>


#3. 시스템 설계
##3.1 시스템 목적

>-기존의 CCTV의 정적인 움직임을 탈피하는 동적인 움직임 구현
-CCTV의 Dead zone을 최소화
-전원, 네트워크 문제시에도 신뢰성 유지
-감시 담당 인력 최소화


####**3.2 시스템 기능**
>-모터 제어 ( 자동 제어, 수동 제어)
- CCTV로부터 물체를 발견했을 때 영상의 이미지 처리와 전송
- 신뢰할 수 있는 데이터 전송 방식
- 긴급 상황에 신호 전송 방식
- 실시간 비디오 Streaming과 비디오 저장
>







####**3.3 전체 시스템 블록 다이어그램**
![image10](http://postfiles7.naver.net/20151211_134/hdhpow_1449813064167pFali_PNG/PIC2079919236.png?type=w1)  

####**3.3.1 시스템 구성**
>**CCTV NODE**
INPUT: 다른 노드의 상태 신호, 수동 제어 신호
OUTPUT: 이미지 처리된 비디오 영상의 데이터, 노드 자신이나 다른 노드의 상태 신호, 다른 노드에게 자신의 신호 전송

>**SERVER**
INPUT: 영상 처리된 실시간 비디오 Streaming 또는 저장된 Streaming, 노드 상태 신호, 수동 제어 신호, 저장된 비디오 Streaming 데이터 요청
OUTPUT: 실시간 Streaming 또는 저장된 Streaming의 상태 정보, 수동 제어 신호

>**CLIENT**
>INPUT: 실시간 Streaming 또는 저장된 Streaming의 상태 정보
OUTPUT: 수동 제어 신호

####**3.3.2 CCTV Node Model**
![image11](http://postfiles3.naver.net/20151211_98/hdhpow_1449813064465cg2VI_PNG/PIC2079919240.png?type=w1)  

>####**구성 및 기능**
-Microprocessor(메인보드)
:입력받은 영상처리 및 각종 디바이스를 제어하는 장치

>-Storage
:네트워크 전송이 불안정 할 때 영상 및 시그널을 저장하는 매체

>-IR LED
:야간에 영상을 획득할 때 추가적 조명에 의해 CCTV_Node 노출될 수 있으나 가시광선 밖의 파형을 가진 IR LED를 장착하여 야간에도 기도비닉을 유지하면서 감시가 가능하도록 한다.

>-Camera
:감시 시 영상을 획득하는 VGA급 해상도의 카메라

>**Network**
:영상 처리 결과 및 상태 정보를 서버로 보내기 위한 네트워크 모듈, 네트워크 상태가 비정상 시에는 시그널을 이웃 CCTV_Node를 통해 전송하도록 하는 WSN(Wireless Sensor Network)를 지원한다. 기본 네트워크망은 고 대역폭의 LTE망을 사용하며 WSN기능을 수행 시에는 Bluetooth를 사용한다. 

>**Servo Motor**
카메라의 Pan, Tilt 동작을 수행하도록 해주는 모터이다. Servo Motor는 DC모터와 다르게 정확한 각도로 움직임을 조절하는 것이 가능하다.

>**Step Motor**
CCTV_Node의 움직임을 담당하는 모터이다. 이 모터는 Servo Motor와 다르게 각도에 제한을 받지 않으며 DC모터와 다르게 정확하게 움직임을 조절하는 것이 가능하다.

>**PWM Circuit**
Servo Motor, Step Motor는 단순히 전압을 공급하는 행위로 동작이 가능하지 않다. 이를 위해서는 특수한 PWM파형을 생성해야한다. Microprocessor에서 자체적으로 생성하는 파형으로는 출력이 부족해 모터를 조작하기 어렵기 때문에 별도의 PWM Circuit을 장착하여 모터를 제어하는 신호를 생성하도록 한다.

>**Power**
:CCTV_Node에 전체적으로 공급되는 전원은 레일의 전선을 통해 공급되는 상시전원과 배터리 전원 두 가지 종류가 있다. 배터리 전원은 평시에는 상시전원을 통해 충전되며 상시전원에 이상이 발생 시 절체 되어 일정 시간동안 CCTV_Node에 전원을 공급하게 된다.

**CCTV Node Function**

![image12](http://postfiles5.naver.net/20151211_116/hdhpow_1449813064728W4yXW_PNG/PIC2085983898.png?type=w1)  

**CCTV NODE**
>INPUT: 다른 노드의 상태 신호, 수동 제어 신호
OUTPUT: 이미지 처리된 비디오 영상의 데이터, 노드 자신이나 다른 노드의 상태 신호, 다른 노드에게 자신의 신호 전송

|**Function**|
|------|
|1 . 움직이는 물체 추적하여 이미지를 캡처하고 처리한다.|
|2 . 데이터를 전송한다.|
|3 . 모터를 제어한다.|

####**3.3.3 Server Model**

![image13](http://postfiles10.naver.net/20151211_73/hdhpow_1449813065108NDaNf_PNG/PIC2085983902.png?type=w1)  

**Server 기능**
![image14](http://postfiles1.naver.net/20151211_16/hdhpow_14498130654111zYWE_PNG/PIC2085983906.png?type=w1)  

**SERVER**
>INPUT: 영상 처리된 실시간 비디오 Streaming 또는 저장된 Streaming, 노드 상태 신호, 수동 제어 신호, 저장된 비디오 Streaming 데이터 요청
OUTPUT: 실시간 Streaming 또는 저장된 Streaming의 상태 정보, 수동 제어 신호
|Function|
|------|
|1 . 비디오 Streaming을 Client에게 전송|
|2 . Client에게 상태신호 전송|
|3 . Client에게 CCTV NODE의 상태정보 전송|
|4 . 데이터를 저장|

####**3.3.4 Client Model**
![image15](http://postfiles14.naver.net/20151211_205/hdhpow_1449813065697cDakR_PNG/PIC2085983910.png?type=w1)  

**Client 기능**
![image16](http://postfiles9.naver.net/20151211_296/hdhpow_1449813065904X0VEJ_PNG/PIC2085983918.png?type=w1)  
**CLIENT**
>INPUT: 실시간 Streaming 또는 저장된 Streaming의 상태 정보
OUTPUT: 수동 제어 신호
|Function|
|------|
|1 . 비디오 Streaming 재생.|
|2 . CCTV로부터 어떤 움직임을 포착했을 때 신호음 발생.|
|3 . 수동 조작.|

####**3.3.5 Motor 제어**
![image17](http://postfiles5.naver.net/20151211_116/hdhpow_1449813066193zRz7m_PNG/PIC2087674282.png?type=w1)  
>자동 조작 : 정해진 스케줄대로 Step Motor과 Servo Motor  
수동 조작 : Client로부터 제어 신호를 받아 수동으로 CCTV NODE를 제어

####**3.3.6 이미지 처리 및 전송**

![image18](http://postfiles11.naver.net/20151211_74/hdhpow_1449813066490I1CQx_PNG/PIC2087674286.png?type=w1)  
|과정|
|------|
|1 . CCTV NODE가 이미지를 캡처 및 처리.|
|2 . 처리된 비디오 Streaming을 Data 전송 모듈에 전송.|
|3 . Server로 Streaming을 전송.|
|4 . Streaming을 Client에 전송.|
|5 . Streaming을 Data Base에 저장|

####**3.3.7 비디오 Playback**
![image19](http://postfiles12.naver.net/20151211_251/hdhpow_1449813066780clrsT_PNG/PIC2087674290.png?type=w1)  
>|과정|
|------|
|1 . Client가 서버로 저장된 비디오 Streaming을 요청|
|2 . 서버는 Database로부터 저장된 비디오를 받음|
|3 . 서버에서 Database로부터 저장된 Streaming을 Client에게 전송.|
|4 . 핵심 컴포넌트 상세 설계|

>이번에 상세 설계하고자 하는 컴포넌트는 CCTV Node의 물체를 탐지하는 부분이다.
물체를 탐지하기 위해서 배경영상과 다음영상의 차이를 이용하여 움직임을 추적하는 차영상 기법을 이용하고 있다. 이러한 영상처리를 위한 클래스를 아래와 같이 설계하였다.


<ObjectDetection Class UML 다이어그램>

이 클래스에 대한 멤버변수와 멤버함수의 기능은 다음과 같다.


#4. 핵심 컴포넌트 상세 설계
>이번에 상세 설계하고자 하는 컴포넌트는 CCTV Node의 물체를 탐지하는 부분이다.
물체를 탐지하기 위해서 배경영상과 다음영상의 차이를 이용하여 움직임을 추적하는 차영상 기법을 이용하고 있다. 이러한 영상처리를 위한 클래스를 아래와 같이 설계하였다.
![image18](http://postfiles12.naver.net/20151211_91/hdhpow_1449813066929DaFt7_PNG/PIC2093297461.png?type=w1)  

##4.1 클래스
####4.1.1 멤버변수

>src_img : 가로 640, 세로 480 해상도로 구성되어 있는 3-byte-channel image matrix
           (취득한 이미지 및 최종 물체 탐색 이미지를 저장)


>gray_binary_img : 가로 640, 세로 480 해상도로 구성되어있는 1-byte-channel 
                   image matrix (src_img의 흑백영상, 차영상, 이진화영상 저장)


>bg_img : 가로 640, 세로 480 해상도로 구성되어있는 1-byte-channel image matrix
          (차영상의 기준이 되는 배경이미지 저장)


>rotated_rect : 탐지된 물체들의 영역을 표시하는 회전 사각형 객체를 저장한는
              vector템플릿 자료구조

>video_capture : 카메라 디바이스의 H/W 동작을 담당하는 디바이스 추상화 객체

>status : 물체 탐지 여부를 확인하는 bool 변수

####4.1.2 멤버함수

>src_img_acquistion : 카메라 디바이스를 동작 시켜 한 프레임의 이미지를 획득 후
                    멤버변수인 src_img에 저장

>bg_img_acquistion : 카메라 디바이스를 동작 시켜 한 프레임의 이미지를 획득 한 후 
                    그레이 스케일로 변환 후 bg_img에 저장해 배경이미지를 얻음

>rgb_to_gray : 매개변수로 원본 이미지 매트릭스 객체와 변환 후 저장될 이미지 매트릭스                 객체를 받는다. RGB영상을 그레이 스케일로 변환하는 역할을 한다.

>abs_diff_img : bg_img와 gray_binary_img를 차영상한 결과 값을 gray_binary_img에 
              저장시키는 함수

>binarization : gray_binary_img로 입력된 그레이 스케일 이미지를 Threshold를 기준으로 
             이진화(0, 255)시켜 gray_binary_img에 저장한다.

>find_moving_object_area_rect : 이진화된 gray_binary_img를 입력받아 움직이는 물체를 탐지하고 물체의 크기가 특정 Threshold 이상인 물체의 외곽선을                          둘러싸는 Rotated rectangles를 구하여 vector타입의                                      rotated_rect 객체에 자료를 추가하는 함수.

>draw_moving_object : src_image에 구한 움직이는 물체를 둘러싸는 rotated_rect를 
                     src_image에 그리는 함수.

>get_src_img_matrix : 다른 클래스에서 이 함수를 호출하여 최종 처리된 src_img를 
                    받아갈 수 있도록 한다.

>get_status : status 변수의 값을 반환하는 함수.

>clear_object : 다음 프레임 촬영을 위해 각 이미지 매트릭스 및 rotated_rect를 
             초기화 하는 함수.


####**4.1.3 수도코드**

```
//src_img_acquistion
video_capture.open(); //카메라 디바이스 open
video_capture.get_frame(src_img); //카메라에서 영상을 src_img에 입력
```
```
>//bg_img_acquistion
video_capture.open(); //카메라 디바이스 open
video_capture.get_frame(bg_img); //카메라에서 영상을 bg_img에 입력
rgb_to_gray(bg_img, bg_img); //bg_img의 영상을 흑백으로 변환

```
```
rgb_to_gray (src, dst)
for(int i = 0; i < 480; I++)
   for(int j = 0; j < 640; j++)
      dst(j,i) = src(i,j,R)/3 + src(i,j,G)/3 + src(i,j,B)/3;
       //dst에 src의 r,g,b 채널의 평균값을 대입(카메라 해상도 640*480)

>channel_set(dst, GRAY_CHANNEL); 
//dst의 컬러채널 수를 1로 설정(잘못된 액세스 방지)
```

```
//abs_diff_img
rgb_to_gray(src_img, gray_binary_img); 
//src_img를 그레이 스케일화 한 결과 값을gray_binary_img에 저장
for(int i = 0; i < 480; I++)
   for(int j = 0; j < 640; j++)
      gray_binary_img(j,i) = abs(bg_img(j,i) - gray_binary_img(j,i)); 
       //배경과 그레이 이미지의 차의 절대값을 그레이 이미지에 저장
```
```
//binarization
for(int i = 0; i < 480; i++)
   for(int j = 0; j < 640; j++) {
      if(gray_binary_img(j,i) < THRESH_VALUE)
         gray_binary_img(j,i) = 0;
      else
         gray_binary_img(j,i) = 255;
   }
//그레이 스케일 이미지의 각 화소값이 특정 THRESH_VALUE을 넘으면 255로 화소값 설정
//넘지 못하면 0으로 화소값 설정을 통해 영상을 이진화 시킴
```

```
//find_moving_object_area_rect
Point_array contour; //외곽선 정보를 저장하는 배열선언
findcontour(gray_binary_img, contour, THRESH_AREA_VALUE);
//이진화 이미지의 일정 면적 이상을 갖는 물체의 외곽선만 탐지한다.
for(int i = 0; i < contour.size(); i++) {
   RotatedRect temp;
   get_contour_min_area_rect(contour[i],temp);
   rotated_rect.push_back(temp); 
}
//찾아낸 물체의 외곽선들의 개수만큼 각 외곽선을 둘러싸는 최소 크기의 회전 사각형 객체를 구하여 rotated_rect에 저장하는 함수.
```


```//draw_moving_object
for(int i = 0; i < rotated_rect.size(); i++) {
   draw_rotated_rect(src_img, rotated_rect[i], RED_COLOR);
}
if(rotated_rect.size() > 0) 
   status = true;
//구한 rotated_rect들을 src_img에 적색으로 그린 다음, 만약 탐지된 물체가 있을 경우 status를 true로 설정하는 함수.
```

```
//get_src_img
return src_img;
//private로 지정된 src_img를 반환하는 함수.
```

```
//get_status
return status;
//private로 지정된 status를 반환하는 함수
```

```
//get_status
memset(&src_img, 0, sizeof(src_img)); //src_img의 메모리 초기화
memset(&bg_img, 0, sizeof(bg_img)); //bg_img의 메모리 초기화
rotated_rect.clear(); // rotated_rect에 저장된 회전 사각형들을 제거
//다음 촬영을 위해 객체의 값을 초기화 하는 함수.
```