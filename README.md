
## Django + Postgres + Docker Compose

This repo contains the sample application for containerising Django app with Postgres using Docker and Docker Compose.

Notice: This sample repo is intended to support a blog post published in the official Docker blogging site. As such, the application code is purposely kept simple to keep the focus on the guide's content and should not be considered production-ready.

### 1. Clone the repository

 ```bash
  https://github.com/dockersamples/django-postgres-docker
 ```


### 2. Navigate to the project directory:

```
cd django-postgres-docker
```

## 3. Create an .env file


```
DJANGO_SECRET_KEY=your_secret_key
DEBUG=True
DJANGO_LOGLEVEL=info
DJANGO_ALLOWED_HOSTS=localhost
DATABASE_ENGINE=postgresql_psycopg2
DATABASE_NAME=dockerdjango
DATABASE_USERNAME=dbuser
DATABASE_PASSWORD=dbpassword
DATABASE_HOST=db
DATABASE_PORT=5432
```

## 4. Bring up the application

```
docker compose up -d --build
```

This command will download any necessary Docker images, build the project, and start the containers. 

<img width="584" alt="image" src="https://github.com/user-attachments/assets/09745514-7bac-4f19-9113-9025cc3bd739">



Once complete, your Django application should be accessible at `http://localhost:8000`.

<img width="993" alt="image" src="https://github.com/user-attachments/assets/583b2085-0e8d-4871-b493-e9726d0a44da">




## Maintenance Schedule
This repo is maintained frequently. For any security updates, note that there may be delays in applying recent fixes.

## License
This project is licensed under the [Apache 2.0 License](/LICENSE).

## Contributing

Since this project is intended to support a specific use case guide, contributions are limited to bug fixes or security issues. If you have a question, feel free to open an issue!
