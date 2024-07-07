# Django Project Templates

Welcome to the Django Project Templates repository! This repository contains a collection of Django project templates designed to help you get started quickly with different types of projects. Whether you're building an e-commerce site, a blog, or a microservice-based application, you'll find a suitable template here.

## Getting Started

To use a template from this repository, follow these steps:

### 1. Create a New Repository on GitHub

1. Go to [GitHub](https://github.com) and create a new empty repository.
2. Copy the URL of the new repository (e.g., `https://github.com/your-username/new-repo.git`).

### 2. Clone the Template Repository

1. Clone the template repository to your local machine:
    ```bash
    git clone --branch branch_name --single-branch https://github.com/BeeCont/django-project-templates.git
    cd template-repo
    ```

### 3. Update Remote Origin

1. Remove the existing remote reference:
    ```bash
    git remote remove origin
    ```

2. Add your new repository as the remote origin:
    ```bash
    git remote add origin https://github.com/your-username/new-repo.git
    ```

### 4. Push to Your New Repository

1. Push the local repository to your new GitHub repository:
    ```bash
    git push -u origin main
    ```

### 5. Switch to the Appropriate Branch

1. If you need to use a specific branch for a template:
    ```bash
    git checkout -b new-branch-name
    git push -u origin new-branch-name
    ```

## Available Templates

Here is a list of available templates, along with their descriptions:

<!--### Main Branch
- **Basic Django Project**: A minimal Django project setup.
-->
### ecommerce-microservice-docker-postgres-poetry-restapi
- **E-commerce Microservice**: A template for an e-commerce site using microservices architecture with Docker, PostgreSQL, Makefile, Poetry.

<!--## Contributing

We welcome contributions! Please read our [Contributing Guide](CONTRIBUTING.md) to learn how you can contribute to this repository.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

Feel free to reach out if you have any questions or need assistance:

- **Email**: [your-email@example.com](mailto:your-email@example.com)
- **GitHub**: [your-username](https://github.com/your-username)
-->
Happy coding!