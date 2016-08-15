# 시작하기

1. [link] (https://github.com/djangogirlscodecamp/djangocupcakeshop) 오른쪽 위에 있는 Fork 버튼을 누르고 git clone을 사용하여 여러분의 컴퓨터에 코드를 복사합니다!

![](clone_djangocupcake.png)

```bash 
$ git clone https://github.com/<user_name>/djangocupcakeshop.git

```
  > 주의: `user_name` 이 부분에 여러분의 Github username을 적어주세요. 여러분의 레파지토리에 fork 되어야 해요!

2. Mac/Linux 환경에서는 terminal, window 환경에서는 prompt을 열고 djangocupcakeshop 폴더로 이동합니다!

```cd djangocupcakeshop ```

3. 아래 command를 콘솔에 치고 가상환경을 만들어야 해요!

#### 윈도우의 경우 
```C:\Python35\python -m venv myvenv``` 
#### 맥의 경우 
```python3 -m venv myvenv ```
#### 리눅스의 경우 : 
```virtualenv --python=python3.4 myvenv```

4. 가상환경을 활성화 시켜 볼까요? 

#### 윈도우의 경우
```bash
myvenv\Scripts\activate 
```
#### 맥이나 리눅스의 경우 
```$ source myvenv/bin/activate ```

터미널 또는 prompt에서 다음과 같이 보이는지 확인해 보세요!

```bash 
(myvenv)... 
```

5. 아래 명령어를 이용해서 필요한 요소들을 설치합니다!

```bash
$ pip install -r requirements.txt
```

6. 다음 명령어를 쳐서 데이터베이스를 만듭니다!

```bash
$ python manage.py migrate
```
[데모를 4(b)](https://djangogirlsseoul.gitbooks.io/-djangocupcakeshop/content/demo.html) 단계 부터 따라 해볼까요!
