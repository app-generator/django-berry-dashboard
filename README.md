# [Django Berry Dashboard](https://appseed.us/product/berry-dashboard/django/)

Open-source **[Django Dashboard](https://appseed.us/admin-dashboards/django/)** crafted on top of **Berry Dashboard**, an open-source `Boostrap 5` design from `CodedThemes`. The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. `Berry` has an easy and intuitive responsive design whether it is viewed on retina screens or laptops.

- 👉 [Django Berry](https://appseed.us/product/berry-dashboard/django/) - `Product page`
- 👉 [Django Berry](https://django-berry.onrender.com) - `LIVE Demo`

<br />

## Features

> `Have questions?` Contact **[Support](https://appseed.us/support/)** (Email & Discord) provided by **AppSeed**

| Free Version                          | [PRO Version](https://appseed.us/product/berry-dashboard-pro/django/)    | [Custom Development](https://appseed.us/custom-development/) |  
| --------------------------------------| --------------------------------------| --------------------------------------|
| ✓ **Django 4.2.9**                    | **Everything in Free**, plus:                                         | **Everything in PRO**, plus:         |
| ✓ Best Practices                      | ✅ **Premium Bootstrap 5 Design**                                     | ✅ **1mo Custom Development**       | 
| ✓ Bootstrap 5, `Material` Design      | ✅ `OAuth` Google, GitHub                                             | ✅ **Team**: PM, Developer, Tester  |
| ✓ `CI/CD` Flow via Render             | ✅ `API`, **Charts**                                                  | ✅ Weekly Sprints                   |
| ✓ `Docker`                            | ✅ **DataTables** (Filters, Export)                                   | ✅ Technical SPECS                  |
| -                                     |✅ **Celery**                                                          | ✅ Documentation                    |
| -                                     | ✅ **Media Files Manager**                                            | ✅ **30 days Delivery Warranty**    |
| -                                     | ✅ **Extended User Profiles**                                         |  -                                   |
| -                                     | ✅ `Private REPO Access`                                              |  -                                   |
| -                                     | ✅ **PRO Support** - [Email & Discord](https://appseed.us/support/)   |  -                                   |
| -                                     | ✅ Deployment Assistance                                              |  -                                   |
| ------------------------------------  | ------------------------------------                                                           | ------------------------------------|
| ✓ [LIVE Demo](https://django-berry.onrender.com)  | 🚀 [LIVE Demo](https://django-berry-pro.onrender.com) | 🛒 `Order`: **[$3,999](https://appseed.gumroad.com/l/rocket-package)** (GUMROAD) |   

![Berry Bootstrap 5 - Dark-Mode ready, Open-source Template.](https://user-images.githubusercontent.com/51070104/215728710-d1ee7fef-8153-402b-9741-371e1c01cd36.png)

<br />

## Manual Build 

> 👉 Download the code  

```bash
$ git clone https://github.com/app-generator/django-berry-dashboard.git
$ cd django-berry-dashboard
```

<br />

> 👉 Install modules via `VENV`  

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

## Codebase structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                            
   |    |-- settings.py                  # Project Configuration  
   |    |-- urls.py                      # Project Routing
   |
   |-- home/
   |    |-- views.py                     # APP Views 
   |    |-- urls.py                      # APP Routing
   |    |-- models.py                    # APP Models 
   |    |-- tests.py                     # Tests  
   |    |-- templates/                   # Theme Customisation 
   |         |-- includes                # 
   |              |-- custom-footer.py   # Custom Footer      
   |     
   |-- requirements.txt                  # Project Dependencies
   |
   |-- env.sample                        # ENV Configuration (default values)
   |-- manage.py                         # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

## How to Customize 

When a template file is loaded in the controller, `Django` scans all template directories starting from the ones defined by the user, and returns the first match or an error in case the template is not found. 
The theme used to style this starter provides the following files: 

```bash
# This is saved in ENV: LIB/admin_berry
< UI_LIBRARY_ROOT > 
   |
   |-- templates/                     # Root Templates Folder 
   |    |          
   |    |-- accounts/       
   |    |    |-- login.html           # Sign IN Page
   |    |    |-- register.html        # Sign UP Page
   |    |
   |    |-- includes/       
   |    |    |-- footer.html          # Footer component
   |    |    |-- sidebar.html         # Sidebar component
   |    |    |-- navigation.html      # Navigation Bar
   |    |    |-- scripts.html         # Scripts Component
   |    |
   |    |-- layouts/       
   |    |    |-- base.html            # Masterpage
   |    |    |-- auth_base.html       # Masterpage for Auth Pages
   |    |
   |    |-- pages/       
   |         |-- index.html           # Dashboard page
   |         |-- color.html           # Colors Page
   |         |-- *.html               # All other pages
   |    
   |-- ************************************************************************
```

When the project requires customization, we need to copy the original file that needs an update (from the virtual environment) and place it in the template folder using the same path. 

> For instance, if we want to **customize the footer.html** these are the steps:

- ✅ `Step 1`: create the `templates` DIRECTORY inside the `home` app
- ✅ `Step 2`: configure the project to use this new template directory
  - `core/settings.py` TEMPLATES section
- ✅ `Step 3`: copy the `footer.html` from the original location (inside your ENV) and save it to the `home/templates` DIR
  - Source PATH: `<YOUR_ENV>/LIB/admin_berry/includes/footer.html`
  - Destination PATH: `<PROJECT_ROOT>home/templates/includes/footer.html`

> To speed up all these steps, the **codebase is already configured** (`Steps 1, and 2`) and a `custom footer` can be found at this location:

`home/templates/includes/custom_footer.html` 

By default, this file is unused because the `theme` expects `footer.html` (without the `custom_` prefix). 

In order to use it, simply rename it to `footer.html`. Like this, the default version shipped in the library is ignored by Django. 

In a similar way, all other files and components can be customized easily.

<br />

## Deploy on [Render](https://render.com/)

- Create a Blueprint instance
  - Go to https://dashboard.render.com/blueprints this link.
- Click `New Blueprint Instance` button.
- Connect your `repo` which you want to deploy.
- Fill the `Service Group Name` and click on `Update Existing Resources` button.
- After that your deployment will start automatically.

At this point, the product should be LIVE.

<br />

## [PRO Version](https://appseed.us/product/berry-dashboard-pro/django/)   

This design is a pixel-perfect [Bootstrap 5](https://www.admin-dashboards.com/bootstrap-5-templates/) Dashboard with a fresh, new design inspired by Google's Material Design. `Material Dashboard 2 PRO` is built with over 300 frontend individual elements, like buttons, inputs, navbars, nav tabs, cards, or alerts, giving you the freedom of choosing and combining.

> Features: 

- `Up-to-date Dependencies`
- `Design`: [Django Theme Berry](https://github.com/app-generator/django-admin-berry-pro) - `PRO Version`
- `Sections` covered by the design:
  - **Admin section** (reserved for superusers)
  - **Authentication**: `Django.contrib.AUTH`, Registration
  - **All Pages** available in for ordinary users 
- `Docker`, `Deployment`:
  - `CI/CD` flow via `Render`

<br />

![Berry Bootstrap 5 PRO - Premium Template Django Template.](https://user-images.githubusercontent.com/51070104/210833058-be0b3e87-4f2b-4765-b84d-3795ba03c6a1.jpg)

<br />

---
[Django Berry Dashboard](https://appseed.us/product/berry-dashboard/django/) - Minimal **Django** starter provided by **[AppSeed](https://appseed.us/)**
