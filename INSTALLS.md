# 설치 정보
## 파이썬 가상환경
### 윈도우 10
#### [아나콘다]
[아나콘다 다운로드](https://www.anaconda.com/download/)
### 우분투 18.04LTS
#### [Pyenv-Virtualenv](https://github.com/pyenv/pyenv-virtualenv)
1. 설치
```bash
# 필수 패키지 설치
sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev \
libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev \
xz-utils tk-dev libffi-dev liblzma-dev python-openssl

# Pyenv 설치
curl https://pyenv.run | bash
```
2. 환경변수 확인(`vim ~/.bashrc`)
```bash
export PYENV_ROOT="$HOME/.pyenv
export PATH="$PYENV_ROOT/bin:$PATH
if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi
```
2-1. 위가 등록되어있지 않을 경우
```bash
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bash_profile
```
3. 터미널 종료 후 다시 시작
## [Source Code Pro](https://github.com/adobe-fonts/source-code-pro)
### 윈도우 10
1. [폰트 다운로드](https://github.com/adobe-fonts/source-code-pro/releases/tag/2.030R-ro%2F1.050R-it)
2. 압축 풀기
3. 제어판 &rarr; 글꼴 &rarr; 드래그

[윈도우10 폰트 글꼴 추가 하는 방법](https://extrememanual.net/6963)
### 우분투 18.04LTS
1. [폰트 다운로드](https://github.com/adobe-fonts/source-code-pro/releases/tag/variable-fonts)
2. 이하 코드
```bash
tar -xvzf source-code-pro-variable-fonts.tar.gz    # 압축 풀기
sudo mkdir /usr/share/fonts/opentype/    # opentype 폴더 생성
mv source-code-pro-variable-fonts /usr/share/fonts/opentype/    # 폰트 옮기기
sudo fc-cache -f -v    # 폰트 등록
```
