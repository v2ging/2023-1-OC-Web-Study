1주차 

- Web 소개
    - 주소
        - Resource가 저장된 주소
        - URI(Uniform Resource Identifier): 리소스를 식별하는 통일된 방식
        - URL(Uniform Resource Location) : 프로토콜(통신규약) + DNS 주소
        - URN(Uniform Resource Name) : 이름으로 찾기
    
    - DNS(Domain Name Server) 등장
        - 길고 복합한 IP 주소를 외우거나 관리하기 힘듦
        - IP 주소는 바뀔 수도 있음
        - Domain Name: 사이트에 이름을 지어줌
        - DNS: 도메인 네임을 한 곳에 저장해 둔 서버
        
    - 서버
        - 자료를 나눠주기 위한 컴퓨터
    
    - 랜더링: HTML, CSS, JS를 재료 삼아 브라우저가 그림을 그려줌
        - HTML: 자료(뼈대)
        - CSS: UI(살, 옷)
        - JavaScript: 제어체계
        
        
2주차

- Git?
    - 컴퓨터파일의 변경사항을 ‘추적’을 작업 ‘협업’을 조율함
    - Git 명령어
        - git add
            - git add 파일명 : ‘파일명’의 이름을 가진 파일을 Staging Area로 이동
            - git add . : 현재 directory의 모든 파일을 Staging Area로 이동
            - git add -A : 수정된 파일 전부 Staging Area로 이동
        - git commit
            - Staging의 파일들 Repository에 commit 하기
            - git commit -m “메시지 입력하기” : -m은 메세지의 약자이고, 뒤의 “ “ 안에 공유할 메세지의 내용을 적음
        - git push
            - 내 로컬 디렉토리(local directory)로 부터 원격저장소(Remote repository)로 보내기 위해 사용 commit 반영하기
            - git push 원격저장소 브랜치: 원격저장소의 브랜치에 푸쉬
        - git log
            - 커밋 이력 확인
            - git log —oneline 한 줄로 요약해서 보고 싶을 때 사용
        
        클론 저장소(clone repository)란?
        
        : 원격 저장소를 복제한 저장소. 이는 다른 사람의 소스 코드 복사본을 생성하는 것과 같으며, 개발을 할 때 우리는 보통 클론 저장소에서 작업을 진행함. 원격 저장소에 변경 사항이 생겼다면, 그 내용을 가져와 클론 저장소를 최신 상태로 유지해주어야 함.
        
        - 다른 사람이 원격저장소에 업데이트한 파일이 있을 때, 원격저장소와 내 로컬저장소의 상태를 동일하게 만들기 위해 사용하는 명령어
            - git pull
                - 원격 저장소에서 변경된 메타데이터 정보를 확인할 뿐 아니라 최신 데이터를 복사하여 로컬 Git에 가져옴
            - git fetch
                - 원격 저장소에 변경 사항이 있는지 확인’만’하고, 변경된 데이터를 로컬 Git엣 실제로 가져오지는 않음
    
    - GitHub(중앙관리자) == remote repository (서버)
        - GitHub desktop 사용시, 편리하게 repository 생성, 관리 가능

- Branch (분기)
    - : 기존코드 변화 -> 새로운 버전
        
         Branch 기능(?)
        
        분기 나누기
        
        분기 합치기
        
        변화 추적(버전 관리)
        
        특정 시점으로 되돌리기
        

- 내 컴퓨터 안에서 일어나는 일
    
    1. 작업공간 / 2. staging area / 3. local repository
    
    1. 내가 작업하는 공간 - 코드들이 작성되는 공간
    2. 코드를 논리적으로(역할별로) 끊어주기 위해 존재 / 코드 잠시 대기시킴
    3.  깃에서 관리하는 저장소
