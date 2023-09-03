> 👉 **Step 1** - Create `.env` file

```bash
$ cd api-server-django 
$ cp env-sample .env
$ nano .env
```

<br />

> 👉 **Step 2** - Build the app

```bash
$ docker-compose up --build 
```

<br />

> 👉 **Step 3** - Migrate DB

```bash
$ docker-compose run --rm pets-app python manage.py makemigrations
$ docker-compose run --rm pets-app python manage.py migrate
```

> 👉 **Step 3** - Create super user

```bash
$ docker-compose run --rm pets-app python manage.py createsuperuser
```


> 👉 **Step 4** - Access it

`http://127.0.0.1:3000` for the react web app
<br />
`http://127.0.0.1:8000` for the python admin page