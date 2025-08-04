## Task 1: Automate Code Deployment Using CI/CD (GitHub Actions)


In this task, I created a simple Node.js web application and set up a CI/CD pipeline using GitHub Actions. The goal is to automatically build a Docker image and push it to DockerHub whenever I push code to the `main` branch.

## Tools Used

- Node.js (Express.js)
- GitHub
- GitHub Actions
- Docker
- DockerHub

##  What I Did

1. Created a simple Node.js app using Express.
2. Wrote a `Dockerfile` to containerize the app.
3. Set up a GitHub Actions workflow to:
   - Install dependencies
   - Run a basic test
   - Build Docker image
   - Push image to DockerHub

The pipeline runs every time I push to the `main` branch.

##  GitHub Secrets Used

I added the following secrets in the GitHub repo:

- `DOCKER_USERNAME` – My DockerHub username
- `DOCKER_PASSWORD` – My DockerHub password or access token

These are used inside the GitHub Actions workflow to log in and push the image.

##  DockerHub Image

After the pipeline runs, the Docker image is available on DockerHub

I pulled the image from DockerHub and ran it.
Then I accessed the app in my browser using:: http://localhost:3000

