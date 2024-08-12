**MySQL**은 오라클 사에서 제공하는 데이터베이스 관리 소프트웨어로, 대용량의 데이터를 관리하고 운영하는 기능을 제공.
1994년에 개발 시작, 2010년에 선마이크로시스템즈 사에 인수, 같은 해에 선마이크로시스템즈 사가 오라클 사에 인수됨.  
MySQL은 교육용이나 개인에게는 무료로 제공됨(무료 에디션). 영리를 목적으로 사용한다면 정해진 비용을 지불해야함(상용 에디션). 상용 에디션은 Standard, Enterprise, Cluster CGE 3개.  
상용 목적인데 무료로 사용하고 싶다면 오픈 소스로 제공되는 MariaDB 사용 권장.

# MySQL 설치를 위한 컴퓨터 환경
설치할 하드웨어에는 윈도우즈(Windows)만 설치되어 있다면 특별한 제한은 없음. 윈도우즈 운영 체제는 64bit Windows 10(또는 11)이 설치되어 있어야 함. 설치하기 전에 컴퓨터의 사양 및 운영 체제를 확인.
1. [시작] 버튼을 마우스 오른쪽 버튼 클릭, [시스템] 선택.
2. 설치된 RAM 등을 확인할 수 있음. [에디션]과 [시스템 종류] 확인. Windows10(또는 11)에 64비트 운영 체제면 설치 가능 환경.

# MySQL 다운로드 및 설치
## MySQL 8.0 최신 버전 다운로드
1. MySQL 다운로드 사이트인 https://dev.mysql.com/downloads/windows/installer/8.0.html에 접속. mysql-installer-community-8.0.21.0.msi 파일의 [Download] 버튼 클릭. 크기는 400MB가 조금 넘음.
2. MySQL Community Downloads 화면이 나타나면 좌측 하단의 [No thanks, just start my download.] 클릭, 다운로드. (로그인 하지 않아도 다운로드 가능)
3. 웹 브라우저 하단에 다운로드가 완료되었다는 메시지 창이 나타남. 실행, 폴더 열기, 다운로드 보기가 가능. [폴더 열기] 버튼을 클릭해서 다운로드된 파일 확인. (다운로드한 파일은 파일 탐색기(windows + e)를 실행해 [내 PC]-[다운로드] 폴더에서 확인 가능)

## MySQL 설치
1. 다운로드한 파일을 더블 클릭해서 설치 시작. 사용자 계정 컨트롤 창이 나타나면 [예] 버튼 클릭.
2. MySQL Installer 창이 나타남. [Choosing a Setup Type]에서는 설치 유형을 선택 가능. 필요한 것들만 골라서 설치하기 위해 'Custom'을 선택하고 [Next] 버튼 클릭.
3. [Select Products and Features]에서 설치할 제품들 선택 가능. [Available Products:]에서 [MySQL Servers]-[MySQL Server]-[MySQL Server 8.0]-[MySQL Server 8.0.21 - X64]를 선택 ->버튼 클릭.
4. [MySQL Workbench 8.0.21 - X64], [Samples and Examples 8.0.21 - X86] 도 추가. Check Requirments 창이 나타나면 [Execute] 버튼을 클릭해서 필요한 부분의 설치 진행. Microsoft Visual C++ 2015 Redistributable을 설치하는 부분인데, 이미 [Windows 업데이트]를 수행했다면 이 부분은 생략될 수 있음.
5. [TCP/IP]가 체크된 상태에서 [Port]가 '3306'인 것을 확인함. [Open Windows Firewall ports for network access]도 체크되어야 함. [Next]버튼 클릭.
6. 파이썬과의 연동을 원활하게 하기 위해 'Use Legacy Authentication Method'를 선택하고 [Next]버튼 클릭.
7. [Accounts and Roles]에서는 MySQL 관리자(Root)의 비밀번호를 설정해야 함. Root는 MySQL의 모든 권한이 있는 관리자의 이름. 비밀번호가 유출되면 컴퓨터의 중요한 정보가 모두 유출될 수 있음. Root의 비밀번호는 문자/숫자/기호를 섞어서 최소 8자 이상으로 만들 것을 권장.
