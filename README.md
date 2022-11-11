# Blackberry

## 개요

이 저장소의 코드들은 블랙베리 교육자료의 예제 소스코드의 예시입니다. 1차시~3차시의 예제 소스코드가 공개되어 있으며\
교육자료에 포함되어 제공하는 전체 예제 소스코드 리스트는 아래와 같습니다.

- 1차시
    - MobileManipulator-Blackberry-01-01-Blink-LED

- 2차시
    - MobileManipulator-Blackberry-02-01-SerialMonitor
    - MobileManipulator-Blackberry-02-02-Monitoring-PSD-Sensor
    - MobileManipulator-Blackberry-02-03-Debugging-PSD-Sensor
    - MobileManipulator-Blackberry-02-04-Monitoring-PSD-Sensor-Bt

- 3차시
    - MobileManipulator-Blackberry-03-01-LED-Digital-Write
    - MobileManipulator-Blackberry-03-02-LED-Analog-Write
    - MobileManipulator-Blackberry-03-03-Button-Digital-Read
    - MobileManipulator-Blackberry-03-04-Buzzer-Tone
    - MobileManipulator-Blackberry-03-05-RGB-LED-Control

- 4차시
    - MobileManipulator-Blackberry-04-01-Gripper-Servo
    - MobileManipulator-Blackberry-04-02-Gripper-Servo2
    - MobileManipulator-Blackberry-04-03-SmartServo-LED

- 5차시
    - MobileManipulator-Blackberry-05-01-MobileBase-One-Wheel
    - MobileManipulator-Blackberry-05-02-MobileBase-Wheels
    - MobileManipulator-Blackberry-05-03-MobileBase-8-Direction
    - MobileManipulator-Blackberry-05-04-MobileBase-Rotation

- 6차시
    - MobileManipulator-Blackberry-06-01-Manipulator-One-Joint
    - MobileManipulator-Blackberry-06-02-Manipulator-Control

- 7차시
    - MobileManipulator-Blackberry-07-01-Forward-Kinematics
    - MobileManipulator-Blackberry-07-02-Inverse-Kinematics

- 8차시
    - MobileManipulator-Blackberry-08-01-Pick-And-Place

- 9차시
    - MobileManipulator-Blackberry-09-01-PSD-distance-calculation
    - MobileManipulator-Blackberry-09-02-PSD-SerialPlotter
    - MobileManipulator-Blackberry-09-03-PSD-Moving-Average-Filter
    - MobileManipulator-Blackberry-09-04-PSD-EWMA

- 10차시
    - MobileManipulator-Blackberry-10-01-IMU-DMP-6Axis
    - MobileManipulator-Blackberry-10-02-IMU-DMP-9Axis

- 11차시
    - 11차시는 소스코드 없이 카메라 소프트웨어 사용법을 학습

- 12차시
    - MobileManipulator-Blackberry-12-01-Pixy2-Basic
    - MobileManipulator-Blackberry-12-02-Pixy2-Manipulator-Tracking

- 13차시
    - MobileManipulator-Blackberry-13-01-Pixy2-Mobilebase-Tracking

- 14차시
    - MobileManipulator-Blackberry-14-01-extended-position-control

- 15차시
    - MobileManipulator-Blackberry-15-01-mission

<br>

## 로봇 구성

Blackberry는 아래 모듈들로 구성됩니다.
- 아두이노 메가 호환보드
- 전방향 구동이 가능한 메카넘 휠(XL430-W250-T 4개)
- 4축 매니퓰레이터(XL430-W250-T 4개)
- Pixy2.1 카메라
- PSD 센서 4개(전방 2개, 좌측 1개, 우측 1개)
- 9축 IMU센서
- 블루투스 모듈
- 사용자 입출력 (부저, RED LED, RGB LED, 택트스위치 2개)

<br>

## 개발환경 셋업

예제 소스코드를 Blackberry에 업로드하여 테스트 하기 위해서는 기본적인 아두이노 개발환경을 설치하고 USB 포트를 통하여 보드와 연결하고 코드를 다운로드 할 준비가 되어 있어야 합니다. 아래에서는 코드를 이 저장소에서 내려받고 아두이노 IDE(개발환경)에서 샘플을 BlackBerry에 다운로드 하는 방법을 설명합니다.\
\
아두이노 IDE를 다운로드하고 설치하는 방법은 다른 인터넷의 많은 가이드들을 참고하기 바랍니다.\
\
모든 코드는 Git 툴을 이용하거나 이 페이지에서 zip 파일로 다운로드 할수 있습니다.
파일목록 바로 위의 버튼들 중 "Code" 를 클릭하고 "Download ZIP" 버튼을 클릭하면 이 코드저장소의 모든 파일을 다운로드 받을 수 있습니다.
PC에서 다운받은 zip 파일을 압축 풀어 둡니다.

<br>

## 펌웨어 다운로드

Blackberry의 후면에는 개발용 PC와 로봇을 연결하기 위한 C타입 USB커넥터가 있습니다. 데이터 통신이 가능한 C타입 USB케이블을 사용해 연결합니다. \
\
로봇에 프로그램을 업로드 할 때는 PC와 로봇이 연결된 상태에서 보드의 좌측면에 보드의 전원 스위치(빨간색)의 흰색 점 부분이 눌려서 보드가 켜진 상태여야 합니다. \
<br>
1. 아두이노 IDE에서 Blackberry 연결을 설정합니다.

    보드 : Arduino Mega or Mega 2560
    
    프로세서 : ATmega2560 (Mega 2560)
    
    포트 : Blackberry와 연결된 시리얼 포트 선택

2. 업로드 버튼을 클릭하여 코드를 빌드하고 Blackberry에 코드를 업로드합니다.

<br>

## 코드 설명

각 예제 프로젝트의 README.md 파일과, 예제 소스코드의 주석을 참고하시기 바랍니다.

<br>

## 모듈 정보
- 스마트 서보 모터 : XL430-W250-T \
manual : https://emanual.robotis.com/docs/kr/dxl/x/xl430-w250
- 블루투스 : HC-06 \
datasheet : https://html.alldatasheet.co.kr/html-pdf/1179032/ETC1/HC-06/109/1/HC-06.html
- PSD : GP2Y0A21YK0F \
datasheet : https://global.sharp/products/device/lineup/data/pdf/datasheet/gp2y0a21yk_e.pdf
- IMU : ICM-20948 \
datasheet, register map : https://invensense.tdk.com/wp-content/uploads/2016/06/DS-000189-ICM-20948-v1.3.pdf
- 카메라 : Pixy2 \
documentation : https://docs.pixycam.com/wiki/doku.php?id=wiki:v2:start

<br>

## 기본 설정값

### 블루투스 모듈
 - 모듈 이름 : RNM0000 (0000부분은 다른 숫자 값일 수 있음)
 - baudrate : 115200
 - password : 1234

<br>

## Pixy2 카메라 관련
Pixy2 카메라는 물체 인식을 위한 시그니처 설정, 카메라 밝기 등의 고급 설정을 위해 PixyMon v2 프로그램을 사용합니다. \
PixyMon v2 프로그램은 아래 링크에서 다운받을 수 있습니다. \
PixyMon v2 다운로드 링크 : https://pixycam.com/downloads-pixy2 \
\
그 외 설정은 Pixy2 문서를 참고해주시기 바랍니다. \
Pixy2 문서 : https://docs.pixycam.com/wiki/doku.php?id=wiki:v2:start \
Pixy2 물체 인식시키기 : https://docs.pixycam.com/wiki/doku.php?id=wiki:v2:teach_pixy_an_object_2 \
PixyMon v2 문서 : https://docs.pixycam.com/wiki/doku.php?id=wiki:v2:pixymon_index