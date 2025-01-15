# Personal DevOps Portfolio Website

A containerized static website showcasing my professional experience and skills as a DevOps Engineer. This project demonstrates various DevOps practices including containerization, CI/CD, and infrastructure as code.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Docker Pulls](https://img.shields.io/docker/pulls/YOUR_DOCKERHUB_USERNAME/resume-website)
![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/YOUR_GITHUB_USERNAME/resume-website/docker-build.yml)

## 🚀 Features

- Responsive static website built with HTML5 and CSS3
- Containerized using Docker
- Automated CI/CD pipeline using GitHub Actions
- Optimized Nginx configuration for static content delivery
- Docker Hub integration for container registry

## 🛠️ Tools Used

- HTML5/CSS3
- Docker
- GitHub Actions
- Nginx
- DockerHub

## 📋 Prerequisites

- Docker installed on your machine
- Git for version control
- GitHub account (for CI/CD)
- Docker Hub account

## 🔧 Local Development

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/resume-website.git
cd resume-website
```

2. Build the Docker image:
```bash
docker build -t resume-website .
```

3. Run the container:
```bash
docker run -d -p 8080:80 resume-website
```

4. Access the website at `http://localhost:8080`

## 🚀 Deployment

The project includes a GitHub Actions workflow that automatically:
1. Builds the Docker image
2. Runs tests
3. Pushes to Docker Hub

To deploy manually:

```bash
# Pull the image
docker pull YOUR_DOCKERHUB_USERNAME/resume-website:latest

# Run the container
docker run -d -p 80:80 YOUR_DOCKERHUB_USERNAME/resume-website:latest
```

## 📁 Project Structure

```
resume-website/
├── .github/
│   └── workflows/
│       └── docker-build.yml
├── index.html
├── styles.css
├── nginx.conf
├── Dockerfile
└── README.md
```

## ⚙️ Configuration

### GitHub Secrets Required
- `DOCKERHUB_USERNAME`: Your Docker Hub username
- `DOCKERHUB_TOKEN`: Your Docker Hub access token

### Nginx Configuration
The project uses a custom Nginx configuration with:
- Gzip compression
- Cache control headers
- Error handling
- Security headers

## 🤝 Contributing

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Contact

- LinkedIn: [Bright Darko Ababio](https://www.linkedin.com/in/bright-ababio)
- Email: darkosloutions@gmail.com

## 🙏 Acknowledgments

- [Nginx Documentation](https://nginx.org/en/docs/)
- [Docker Documentation](https://docs.docker.com/)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)

---
⭐️ Star this repository if you find it helpful!
