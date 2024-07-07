# ecommerce-docker-postgresql-makefile-poetry-template

This project template use Django for the backend, Docker for containerization, Poetry for dependency management, Docker Compose for orchestration, and Makefile for simplifying development tasks.

## Key Technologies

- **Django**: Web framework for backend development.
- **Docker**: Platform for containerizing applications.
- **PostgreSQL**: Open-source object-relational database system.
- **Poetry**: Tool for dependency management and packaging Python projects.
- **Docker Compose**: Tool for orchestrating multi-container Docker applications.
- **Makefile**: Automation of frequently used commands.

## Installation and Setup

1. **Clone the Repository**

```bash
git clone --branch ecommerce-docker-postgresql-makefile-poetry-template --single-branch https://github.com/BeeCont/django-project-templates.git
```

2. **Install Dependencies**

   - Install Poetry if it's not already installed:
      ```bash
      curl -sSL https://install.python-poetry.org | python3 -
      ```
   - Then install the dependencies:
      ```bash
      poetry install
      ```
   
3. **Configure the Environment**

   - Create an env file based on env_example:
      ```bash
      POSTGRES_DB=my_database
      POSTGRES_USER=my_user
      POSTGRES_PASSWORD=my_password
      POSTGRES_PORT=5432
      POSTGRES_HOST=postgres
      DJANGO_PORT=8000
      DJANGO_SECRET_KEY=mysecretkey
      ```

4. **Run the Project**

   - Build and run the project using Docker Compose:
      ```bash
      #Using a Makefile
      make app

      #Without Makefile
      docker compose -f docker_compose/app.yaml -f docker_compose/storages.yaml --env-file env/.env  up --build -d
      ```

## Using Makefile

**Implemented Commands**

* `make app` - up application and database/infrastructure
* `make app-logs` - follow the logs in app container
* `make app-down` - down application and all infrastructure
* `make storages` - up only storages. you should run your application locally for debugging/developing purposes
* `make storages-logs` - foolow the logs in storages containers
* `make storages-down` - down all infrastructure
* `postgres` - сonnect to the database

**Most Used Django Specific Commands**

* `make migrations` - make migrations to models
* `make migrate` - apply all made migrations
* `make collectstatic` - collect static
* `make superuser` - create admin user