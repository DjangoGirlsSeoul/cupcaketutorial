# Getting Started

## Fork and clone this repository for Tutorial

Press the fork button on the top right at this [link](https://github.com/djangogirlscodecamp/djangocupcakeshop).

![](fork_djangocupcakeshop.png)

Use git clone to copy code on your computer.

![](clone_djangocupcake.png)

```bash 
$ git clone https://github.com/<user_name>/djangocupcakeshop.git

```

  > Note: replace <user_name> with your Github username. It should be the forked repository from step 1. 

Open terminal (Mac/Linux) or command prompt (windows) and go to djangocupcakeshop folder 

```cd djangocupcakeshop ```

`cd djangocupcakeshop` 치고 djangocupcakeshop 폴더 안으로 이동

Create a virtual environment by using the command
#### Windows:
```C:\Python35\python -m venv myvenv```
#### Mac:
```bash
$ python3 -m venv myvenv 
``` 
####Linux:
```bash 
$ virtualenv --python=python3.4 myvenv
```

Activate virtual environment by using 
#### windows
```bash
myvenv\Scripts\activate 
```
#### Mac/Linux
```$ source myvenv/bin/activate ```

Confirm it by seeing myvenv appears like this on your terminal/command prompt

```bash 
(myvenv)... 
```

Install django by executing this command 

```bash
$ pip install -r requirements.txt
```

Make database by executing the following command

```bash
$ python manage.py migrate
```

Follow step 4(b) from [demo section](https://djangogirlsseoul.gitbooks.io/-djangocupcakeshop/content/demo.html) onwards

