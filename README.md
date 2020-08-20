# 클레이튼 바오밥 테스트넷 이용해서 Bapp 만들기

## 속전 속결 덧셈 게임
### 환경구축
  - truffle version 4.1.15
  - node version 8 이상
  - nvm 되도록이면 사용해서 관리하자
  - 깃허브 업로드 하기전 .gitignore로 모듈은 항상 가려주자(너무 무거움)
  - VScode
### migrations 폴더에 컨트랙트 배포할수있는 js 파일 생성 및 설정
  - 2_deploy_contract.js 생성 및 deployedABI,deployedAddress 에 자동으로 기입되기위한 함수 작성
  - deployedABI,deployedAddress 파일 생성
### truffle.js 파일 내용 수정
  - 바오밥 네트워크에서 사용할 클레이튼 지갑 개인키
  - 네트워크 아이디
  - 가스 리미트 설정
  - 클레이튼 바오밥 테스트넷 풀노드 작동하는 네트워크 포트 연결
  - require('truffle-hdwallet-provider-klaytn'); //기존의 모듈은 klaytn에서 새로운 모듈로 바꿨으니 주의

### 배포하는 순서

  - truffle deploy --network klaytn ( 배포 )
  - truffle deploy --reset --comfile-all --network klaytn (재 배포 )

### front 작성
  - 진행중
  - aa
