# 3주차 회고


## 충돌 해결하기

degit을 사용하여 추가된 login 파일만 가져오려다가 이번 기회에 충돌에 관해 공부하고자 fetch로 수동 병합을 시도해 보았다. 자동 병합보다 꼼꼼하게 파일을 확인하고 가져올 수 있다는 점이 좋았다! 다음엔 degit을 시도해 봐야겠다.   


## 과제를 하면서.. ⌯ᵔ⩊ᵔ⌯ಣ

### 궁금증

- 눈 모양 로고(비밀번호 노출 여부)는 <input type="checkbox">와<button> 중 어떤 게 더 적절한지.  

### 고민했던 부분과 실행  

로그인 같은 민감한 개인정보를 담은 폼을 어떻게 전달하면 좋을까?  
method ="GET"은 URL에 내 아이디와 비밀번호가 노출되지만, method= "POST"은 노출되지 않는다. 둘 다 개발자 도구에서도 확인이 가능하여 '네트워크' 탭에서'탭에서 이를 확인해 보았다.  

저번엔 <button title="">버튼에 title속성 값을 주었는데, 이번엔 <button> <title>로 정보값을 넣어보았다.  
터치스크린의 경우엔 마우스 오버의 기능을 사용할 수 없고 키보드 만으로 웹페이지를 이용하는 사람들을 고려하여 title을 전역 속성에서 사용하지 않는 게 좋을 것 같다.  

로그인 페이지로 유입된 사람들의 목적은 로그인 or 회원가입 크게 둘로 나뉜다고 생각했으므로, 바로 로그인을 할 수 있는 환경을 만들고자 autofocus 속성을 사용하였다.  

로고를 삽입할 때 <svg> 직접 삽입, <img>로 불러오기, 배경 이미지로 삽입 중 어떤 게 가장 좋을지 고민하였다.   
반응형 디자인이지만 로고는 동일한 크기를 유지하고 있으므로 img로 링크 안에 넣는 방식을 택했다. 배경 이미지로 불러오는 경우엔, 스크린 리더가 읽지 않아도 되는 정보를 담은 이미지만 가져와야 좋을 듯싶다.  

아이디(이메일)이라고 하니, 아이디는 이메일만 된다는건지 아이디와 이메일 모두 된다는 건지 명확하게 이해하기 어려워서 이 부분은 아이디 또는 이메일로 수정하였다.  

폼즈프리를 깔고 어떻게 폼 형식이 도착하는지 확인하려고 회원가입을 했다. 그러나 첫 시도 후 바로 로그인이 막혀버렸다.    
Form has been blocked due to suspected fraudulent activity..  

IP 보안 관련 내용을 보여주기 위해 a 태그, popover, dialog중에 고민하였다. 이번엔 html과 CSS 구성으로만 만들고 싶었고, 굳이 새 탭으로 이동하지 않아도 해당 페이지에서 팝업창처럼 뜨는 형식인 popover를 선택해 보았다.팝업의 내용은 라디오 버튼이 있는 폼 형식이어도 괜찮을까..  

### 시도하였지만 마무리하지 못한…. 진행 상태(─‿─)

- css 스타일링
- 폼 유효성 검사를 실현하기 위해 html의 pattern 속성과 css의 :valid, :invalide 를 시도하였으나..  
- 입력 서식이 공란일 땐 x(초기화)버튼이 보이지 않고, 텍스트 입력 시 보이는 방법  
- ip 보안과 같이 중요한 정보를 담고 있는 경우엔 <strong>으로 사용하여 스크린 리더가 강하게 읽을 필요성이 있는가.  
- 대문자 설정이 켜진 줄 모르고 계속 로그인 시도를 하는 때를 대비해 애초에 대문자 설정을 막는 방법이 맞을지..(보이스 오버로 실험했을 땐 대문자와 소문자를 말할 때 목소리가 다르다.)  


## 이번주 수업 후기 ՞⸝⸝ᵒ̴̶̷ 𓈞 ᵒ̴̶̷⸝⸝՞
3주차는 굉장히 알차고 좋은 정보로 응축된(?) 수업이었다. 가장 재밌었던 부분은 @media, custom properties, aspectio-ration, clamp..  
그리고 하나둘 즐겨찾기에 쌓여가는 유용한 사이트들!!  
