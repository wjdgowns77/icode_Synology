# icode를 통해 시놀로지 NAS에서 문자 발송하기!     
## 소개.    
시놀로지 NAS를 통해 텔레그램 문자를 보내는 방법은 알려져 있으나, 일반 SMS를 보내는 방법은 잘 알려져있지 않아 소개하게 되었습니다. 따로 소스는 없고, 여기 나와있는대로 등록만 하시면 됩니다.    
## 하는방법.
먼저 당연히 icode에 회원가입을 하신 다음 돈을 넣어두셔야 합니다.    
http://www.icodekorea.com/ 이곳에서 회원가입 하시고, 만원쯤 넣어두시면 아마 NAS 고장날때까지 쓸겁니다.    
SMS provider 를 추가한 후 다음과 같이 입력합니다. cp= 부분 빼고는 그대로 복붙하시면 됩니다    
SMS URL= http://www.icodekorea.com/res/sms.php?msg=Hello World&id=myid&pw=mypw&hplist=01012345678&cp=01090123456    
(cp=01090123456 부분은 등록된 발신 전화번호를 적어주셔야 합니다. 제대로 입력 안하시면 진행 안되니 주의하시길 바랍니다.)     
다음 창에서 위 get요청의 상세 사항에 대해 물어보는데, 다음과 같이 선택해 주시면 됩니다.    
    
msg=Hello World	=> Message conetent    
id=myid		=> Username    
pw=mypw		=> Password    
hplist=01012345678=>Phone number    
cp=내전화번호	=> Other    
    
Apply 하시고, 선택사항이 적용되면, 실제 정보를 입력해 줍니다.     
Username에는 icode ID, Password에는 icode PW, Confirm Password에는 icode PW 다시 입력해 주세요.       
Primary Phone number에는 휴대폰 번호를 입력해 주시면 되는데, 첫번째 란 비워두고 두번째 란에 010, 세번째 란에 나머지 입력하시면 됩니다.    
    
Send a test SMS message 해보시고, 약 10초후 휴대폰에서 메시지가 잘 도착하면 어플라이 하시면 됩니다.    
잘 모르시겠다면, 언재나 그렇듯이 이메일 보내시면 도와드립니다 :)
