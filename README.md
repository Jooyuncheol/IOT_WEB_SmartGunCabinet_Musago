





![스크린샷(2)](https://user-images.githubusercontent.com/85000764/190904516-a8c98a30-0ab6-45ae-89d0-8b2ead8666e7.png)







# IOT_SmartGunCabinet_Musago(스마트 총기보관함)

총을 불출하고 반납할때 자동으로 총의 개수을 계산하여 총기현황판을 최신화 해주는 제품입니다.


# 프로젝트소개

 

 - 군인 하면 떠오르는 것은 바로 총입니다. 
실제로 육해공군을 가리지 않고 우리 국군은 군생활을 하며 총을 가장 많이 다룰 것이라 생각합니다. 총은 개인 화기로서 개인에게 지급되어 개인이 관리하는 병기인데 그렇기에 개수 파악 및 현황을 파악하기 위해 각 총기함 마다 총기현황판이 있습니다. 
위병소 근무가 있는 부대 같은 경우는 매일 정해진 시간에 총기 교대를 하고 일반적으로는 훈련 상황일때 총기를 불출합니다. 특히 전투준비태세와 같은 훈련의 경우 시간을 최소화하는 것이 생명인데 현재 사용하고 있는 총기현황판의 경우 직접 수기로 총기 개수를 파악하여 적어야 하기에 많은 시간을 요구하는 동시에 실수를 저지를 확률이 높습니다.  
 따라서 이것을 개개인이 직접 수기로 적는 것이 아닌 간단한 디스플레이를 활용하여 총기의 현황을 최신화 할 수 있는 제품을 고안하였습니다.

## 기능설명



## 기술 스택 (Technique Used)

 - 각총기현황판에 부착할 iot 제품 개발을 목표로 하고 있습니다.  기본적인 구성은 아두이노, nextion 디스플레이, 무게센서 이렇게 세가지 입니다.  
 - nextion 디스플레이가 기존의 총기현황판을 대체하여 정보들을 표시 및 수정을 용이하게 할 것 입니다. 
 - 총기를 불출할시 용사들이 본인의 이름을 터치하고 훈련/근무/출타와 같은 총기 불출 이유를 클릭하면 자동으로 총기 실셈이 되어 정보가 업데이트되는 방법을 구상하였습니다. 
 - 2차 보안으로 무게센서를 각 총기함 아래 부분에 설치하여 터치 오류와 같은 일들을 방지할 수 있습니다.

## 기대 효과 및 전망

 - 스마트 총기보관함을 사용함으로서 기존에 총기를 불출하고 반납할 때 총기 수를 세는데 있어 실수할 수 있는 경우를 없애 줄 것입니다.  
 - 훈련상황, 나아가 실제 상황이 발생하여 일분일초가 긴급한 상황에서 총기 현황판을 수정하는데 시간을 단축시켜주어 출동 준비 시간을 더 신속하고 빠르게 할 수 있습니다. 특히 5분 대기조와 같이 속도가 중요한 경우 스마트 총기보관함 확연한 도움이 될 것입니다.  
 - 비용이 많이 들지 않는 기술로 모든 부대에 설치하기 용이할 것입니다.  
 - 훈련 상황 외에도 병기계원 혹은 당직병들이 총기 실셈을 할때 큰 도움을 줄 것이고 정확한 데이터를 기반으로 하여 체계적인 총기관리가 이루어질 것 입니다.

## 프로젝트 사용법 (Getting Started)

### WEB서비스 설치법  

git 저장소를 복사합니다.  
```$ git clone https://github.com/osamhack2022/IOT_WEB_SmartGunCabinet_Musago```  

복사한 저장소 디렉토리로 이동  
```$ cd IOT_WEB_SmartGunCabinet_Musago```  

setup.sh 스크립트 실행  
```$ sudo sh ./WEB_BE/setup.sh```  

http://127.0.0.1:5000 을 웹브라우져로 열면 서비스 이용이 가능합니다.

### 설정 변경법  

설정 파일이 있는 디렉토리로 이동  
```$ cd $MUSAGO_WEB_BE_HOME```  

설정파일을 편집  
```$ sudo nano config.py```  

서비스 제시작  
```$ sudo systemctl restart sgc_musago```  

### 관련 명령어  

서비스 시작  
```$ sudo systemctl start sgc_musago```  
서비스 종료  
```$ sudo systemctl stop sgc_musago```  
서비스 재시작  
```$ sudo systemctl restart sgc_musago```  

## 팀 정보 (Team Information)

 - 팀장(프로젝트 총 책임자): 신화랑(alceoswr@gmail.com)
 - 임배디드 개발자: 임채주(cjlim000523@gmail.com)
 - WEB-임베디드 개발자: 박제형(sjsanjsrh@naver.com)



## 저작권 및 사용권 정보 (Copyleft / End User License)
 * [MIT](https://github.com/osam2020-WEB/Sample-ProjectName-TeamName/blob/master/license.md)

This project is licensed under the terms of the MIT license.

