> 👉 **Step 1** - Start the APP in `Docker`

```bash
$ docker-compose up --build 
```

<br />

> 👉 **Step 2** - `Migrate DB`

```bash
$ docker-compose run --rm pets-app python manage.py makemigrations
$ docker-compose run --rm pets-app python manage.py migrate
```

<br />

> 👉 **Step 3** - Access the `APP`

Visit `http://127.0.0.1:3000` in your browser. The App should be `up & running`.