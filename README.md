# RabbitVCS HamoniKR Release
===========================

하모니카 파일 탐색기에서 소스코드 버전 관리 도구를 제공하는 프로그램.

RabbitVCS 프로젝트는 사용하는 SVN, GIT, HG 등의 버전 관리 시스템에 대해 사용자에게 동일한 환경을 제공하는 GUI 프로그램입니다.

이 프로젝트는 터미널의 명령행을 이용하지 않고도 파일 탐색기에서 모든 버전 관리 시스템의 작업을 수행할 수 있습니다.

![rabbitvcs](imgs/img-1.png)

![rabbitvcs](imgs/img-2.png)

# Install

## HamoniKR 사용자의 경우
터미널을 열고(Ctrl+Alt+T) 아래 명령어를 입력하세요.

```
sudo apt update
sudo apt install -y rabbitvcs-nemo
```

## Ubuntu, LinuxMint 등 다른 우분투 계열 배포판 사용자의 경우
터미널을 열고(Ctrl+Alt+T) 아래 명령어를 입력하세요.

```
wget -qO- https://pkg.hamonikr.org/add-hamonikr.apt | sudo -E bash -

# nemo 
sudo apt install -y rabbitvcs-nemo

# nautilus
sudo apt install -y rabbitvcs-nautilus

# gedit
sudo apt install -y rabbitvcs-gedit

```

## Manual Install
Execute the following:
```
git clone https://github.com/hamonikr/rabbitvcs-hamonikr.git
cd rabbitvcs-hamonikr

sudo python setup.py install --record installfiles.txt
```

### On Ubuntu or Debian-based distros, instead run:
```
sudo python setup.py install --install-layout=deb --record installfiles.txt

sudo cp -v clients/nemo/RabbitVCS.py /usr/share/nemo-python/extensions/RabbitVCS.py

sudo chmod +x /usr/share/nemo-python/extensions/RabbitVCS.py
nemo -q
```

### uninstall
```
sudo xargs rm -rf < installfiles.txt
sudo rm -f /usr/share/nemo-python/extensions/RabbitVCS.py
```

# Usage
 * 파일 탐색기 실행 후 마우스 오른쪽 메뉴를 누르면 프로그램 메뉴가 나옵니다.
 
 # 이슈 또는 버그
 사용 중 문제를 발견하시면 root@hamonikr.org 또는 https://groups.google.com/forum/m/#!forum/hamonikr 에서 알려주세요.



References
----------
Homepage: http://www.rabbitvcs.org
