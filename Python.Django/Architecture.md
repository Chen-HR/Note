# Django File Architecture

---

## `{Project}/`

- Project content.

## `{Project}/manage.py`

- Project manage tool.
  - Create SQLite Database: `manage.py makemigrations`
  - Synchronize database with models: `manage.py migrations`
  - Start server: `manage.py runserver`

---

## `{Project}/{Project}/`

- Porject Setting, Alloc, Config.

## `{Project}/{Project}/__init__.py`

- Empty file
- Make this folder to `Python Pachage`

## `{Project}/{Project}/settings.py`

- This project setting
  - `DEBUG`: set open Debug mode
  - `INSTALLED_APPS`: The "APP" (module) that will be used to start this project
  - `TEMPLATES[]`: templates config
    - `'DIRS'`: templates folder path list
  - `LANGUAGE_CODE`: language family ('zh-hant')
  - `TIME_ZONE`: timezone ('Asia/Taipei')
  - `STATIC_URL`: Set the static folder in the URL path
  - `STATICFILES_DIRS`: Set the static folder in this file system

## `{Project}/{Project}/asgi.py`

- ASGI server config
- Django interface config

## `{Project}/{Project}/wsgi.py`

- Web server config
- Django interface config

## `{Project}/{Project}/urls.py`

- URL config

---

## `{Project}/templates/`

- HTML template file folder

## `{Project}/templates/`*`.html`

- HTML template file.

---

## `{Project}/static/`

- Static file folder.
- Usually stores files that are less relevant to this `Python.Django` project. E.G. CSS file, JavaScript file, multimedia files(E.G. images, music, video.)

---

## `{Project}/{Application}/`

- Project's Application(run as Python's Module).
- Usually stores files that are less relevant to this `Python.Django` project. E.G. CSS file, JavaScript file, multimedia files(E.G. images, music, video.)
