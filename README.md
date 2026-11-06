# ShopEase

A simple online shopping and order management interface built with HTML, CSS, and JavaScript. Product catalogue, search, cart, checkout, order history, and admin product management are included. Demo data is saved in browser localStorage.

## Run in VS Code

1. Open this folder in VS Code.
2. Open `site/index.html` in a browser, or use the Live Server extension.

## Run with Docker

Install Docker Desktop, open a terminal in this folder, and run:

```powershell
docker compose up --build
```

Then visit http://localhost:8080. Stop it with `Ctrl+C`.

## Jenkins

Create a Jenkins Pipeline job connected to this GitHub repository and select **Pipeline script from SCM**. The pipeline uses the `Jenkinsfile` to check out the code and build a Docker image. The Jenkins agent needs Docker installed and available as `docker` in its Windows command prompt.

## Push to GitHub

Create an empty repository on GitHub, then run these commands from this folder (replace the URL):

```powershell
git init
git add .
git commit -m "Add ShopEase shopping app"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```
