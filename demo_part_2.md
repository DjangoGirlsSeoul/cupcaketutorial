# Demo Part 2
## Step 9 Dynamic data in Templates with ORM [템플릿의 동적 데이터](http://tutorial.djangogirls.org/en/dynamic_data_in_templates/#dynamic-data-in-templates)
>relevant git branch `orm`

a. Get Dynamic data (cupcakes) from database using queryset. Add following code in `menu/views.py` in `cupcake_list` function.

```python
from django.shortcuts import render
from .models import Cupcake

def cupcake_list(request):
    cakes = Cupcake.objects.all().order_by('-createdAt')
    context = {"cakes": cakes}
    return render(request,"menu/list.html",context)
    ```

Above query `Cupcake.objects.all().order_by('-createdAt')` will fetch all the cupcakes from the database in descending order with respect to `createdAt`.

> That code loads the template called menu/list.html and passes it a context. The `context` is a dictionary mapping template variable names to Python objects.

If we visit the home page, we cannot see the data from database in template. Time to go back to our template and display this QuerySet!

b. We will use Django Template Tags to add data from our queryset to template. We will remove the hard-coded cupcakes and replace it with following. 

`list.html`

```html

```
a. 쿼리셋
b. menu 목록 템플릿 보여주기

## Step 10 (프로그램 어플리케이션 확장하기)
	a. menu에 템플릿 링크 만들기 그리고 Rest 상세 페이지에 뷰 추가하기
	b. 다시한번 배포 하기

## Step 11 [배포하기](http://tutorial.djangogirls.org/ko/deploy/#github에서-pythonanywhere로-코드-가져오기)
	a. PythonAnywhere에서 무료 계정인 "초보자(Beginner)"로 회원가입 하세요. GitHub에서 PythonAnywhere로 코드 가져오기
	b. PythonAnywhere에서 가상환경(virtualenv) 생성하기. 콘솔창에서 `virtualenv --python=python3.4 myvenv` 그리고 `pip install -r requirements.txt` 실행하세요.정적 파일 모으기 `python manage.py collectstatic`
	c. PythonAnywhere에서 데이터베이스 생성하기 `python manage.py migrate`
	d. web app으로 DjangoCupcakeshop 배포하기 - 가상환경(virtualenv) 설정하기 그리고 WSGI 파일 설정하기


## Step 12 (Django 폼)
	a. 이제 한 가지만 더 하면 웹사이트가 완성되어요. 바로 식당을 추가하거나 수정하는 멋진 기능을 추가하는 것이죠. 폼과 페이지 링크 만들기
	b. 폼과 링크를 연결하고 저장된 폼에 View 메소드를 추가하기
	c. 폼 보안
	d. 폼 수정하기- 한 가지만 더: 배포하세요

## Step 13 (숙제)
	a. '점수' 목록 배열하기
	b. '가격' 목록 배열하기

## Step 14 (Extended)




