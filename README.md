# CRUD

## 0. setting

- 가상환경 생성
- 가상환경 활성화
- `.gitignore` 설정 (python, window, macOS, Django)

## 1. Django

- `pip install django`

- 프로젝트 생성
```shell
django-admin startproject crud .
```

- 앱 생성 / 등록
```shell
django-admin startapp posts
```

## 2. CRUD

- modeling(`models.py`)

```python
class Post(modles.Model):
    title = models.CharField(max_length=100)
    content = models.TextField()
```

- migration
```shell
# 번역본 생성
python manange.py makemigrations
```

```shell
# DB에 반영
python manage.py migrate
```