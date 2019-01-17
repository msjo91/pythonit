# 가상환경
## Conda
> Anaconda Prompt 열기
```bash
# 버젼 확인
conda --version
# 업데이트
conda update conda
# 파이썬 환경 확인
conda info --envs
conda env list
# 설치 가능한 파이썬 리스트 보기
conda search python
# 가상환경 만들기
conda create --name <가상환경이름> python=<파이썬 버젼>
# 가상환경 켜기
activate <가상환경이름>
# 가상환경 삭제
conda remove --name <가상환경이름> --all
conda env remove --name <가상환경이름>
# 가상환경 정보 저장
conda env export > environment.yml
# 패키지 확인
(가상환경을 activate한 상태로) conda list
# 패키지 설치
(가상환경을 activate한 상태로) conda install <패키지이름>
# 패키지 업데이트
(가상환경을 activate한 상태로) conda update <패키지이름>
# 패키지 삭제
(가상환경을 activate한 상태로) conda uninstall <패키지이름>
```
## Pyenv-Virtualenv
```bash
# 파이썬 환경 확인
pyenv versions
# 설치 가능한 파이썬 리스트 보기
pyenv install --list
# 파이썬 설치
pyenv install <파이썬 버젼>
# 가상환경 만들기
pyenv virtualenv <파이썬 버젼> <가상환경이름>
# 가상환경 적용
pyenv local <가상환경이름>
# 파이썬 환경 삭제
pyenv uninstall <환경이름>
# 패키지 확인
(가상환경이 적용된 디렉토리에서) pip list
# 패키지 업데이트 확인
(가상환경이 적용된 디렉토리에서) pip list --outdated
# 패키지 설치
(가상환경이 적용된 디렉토리에서) pip install <패키지이름>
# 패키지 업데이트
(가상환경이 적용된 디렉토리에서) pip install --upgrade <패키지이름>
# 패키지 삭제
(가상환경이 적용된 디렉토리에서) pip uninstall <패키지이름>
# 패키지 정보 저장
(가상환경이 적용된 디렉토리에서) pip freeze > requirements.txt
```
