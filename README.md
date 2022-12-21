# [Django Berry PRO](https://github.com/app-generator/django-berry-dashboard-pro) `Starter`

**Django** starter styled with **Berry Dashboard PRO**, a premium `Boostrap 5` design from [CodedThemes](https://codedthemes.com/?ref=appseed)
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme. During the purchase, a 


<br />

## Features: 

- ✅ `Up-to-date Dependencies`
- ✅ `Design`: [Django Theme Berry](https://github.com/app-generator/django-admin-berry-pro) - `PRO Version`
- ✅ `Sections` covered by the design:
  - ✅ **Admin section** (reserved for superusers)
  - ✅ **Authentication**: `Django.contrib.AUTH`, Registration
  - ✅ **All Pages** available in for ordinary users 
- ✅ `Deployment-Ready` for Render  
- 🚀 [Support](https://appseed.us/support/) via `Email` & `Discord` 

<br />

![Berry Bootstrap 5 - Dark-Mode ready, Open-source Template.](https://user-images.githubusercontent.com/51070104/207091062-e805b36c-663a-4a01-acb8-9c55ab914f4f.jpg)

<br />

## Manual Build 

> 👉 Download the code  

```bash
$ git clone https://github.com/app-generator/django-berry-dashboard-pro.git
$ cd django-berry-dashboard-pro
```

<br />

> Export `GITHUB_TOKEN` in the environment. The value is provided by AppSeed during purchase. 

This is required because the project has a private REPO dependency: `github.com/app-generator/priv-django-admin-berry-pro`

```bash
$ export GITHUB_TOKEN='TOKEN_HERE'  # for Linux, Mac
$ set GITHUB_TOKEN='TOKEN_HERE'     # Windows CMD
$ $env:GITHUB_TOKEN = 'TOKEN_HERE'  # Windows powerShell 
```

<br />

> 👉 Install modules via `VENV`.


```bash
$ virtualenv env
$ source env/bin/activate
$ pip install -r requirements.txt
```

<br />

> 👉 Edit the `.env` using the template `.env.sample`. 

```env

# True for development, False for production
DEBUG=True

```

<br />

> 👉 Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> 👉 Create the Superuser

```bash
$ python manage.py createsuperuser
```

<br />

> 👉 Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

## Screenshots

![Berry Bootstrap 5 - Sign IN, Open-source Starter by AppSeed.](https://user-images.githubusercontent.com/51070104/207091198-2753246e-3d65-4aac-96de-0598a9a94788.jpg)

<br />

> [Django Admin Berry](https://github.com/app-generator/django-admin-berry) - `Icons` Page

![Berry Bootstrap 5 - UI Icons page, Open-source Starter by AppSeed](https://user-images.githubusercontent.com/51070104/207091655-d5005e08-7ea0-4367-ab3a-2cd16934d2fd.jpg)

<br />

> [Django Admin Berry](https://github.com/app-generator/django-admin-berry) - `Colors` page

![Berry Bootstrap 5 - Colors page, Open-source Starter by AppSeed](https://user-images.githubusercontent.com/51070104/207091441-942be542-2794-4bdb-a51d-85c75b5bc692.jpg)

<br />

---
[Django Berry Dashboard](https://github.com/app-generator/django-berry-dashboard-pro) - Minimal **Django** starter provided by **[AppSeed](https://appseed.us/)**
