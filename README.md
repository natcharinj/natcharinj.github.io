# gatsby-starter-minimal-portfolio

## Prerequisite
- Computer (Windows or Linux based OS)
- Node
- Yarn
- Git
- GitHub Account for deploying to GitHub Pages 

## Create and run a new project
- Create a new project from gatsby-starter-minimal-portfolio.
  ```sh
  gatsby new {your-github-username}.github.io dotnetthailand/gatsby-starter-minimal-portfolio
  ```
- Wait for a while until cline has finished.
- CD to your project folder.
  ```sh
  cd {your-github-username}.github.io
  ```
- Run your project.
  ```sh
  yarn start
  ```
- Open a browser and navigate to http://localhost:8000.
- You will find your minimal-portfolio in a browser.
- Optionally, run `code .` to open a project with VS Code.

## Customize your portfolio
- Edit content of `SiteConfig.js` to your profile information.
- Add a new Markdown file in `content` folder and put your activity's details into it.
- Edit `data/projects.yml` to your interesting projects.
- Edit content of `src/pages/contact.tsx` to your contact information (We use Gatsby theme shadowing).
- Kill a process with yarn `ctrl+c` and start it over again with `yarn start`.

## Deploy to GitHub Pages
- Create an empty repository with a name as `your-github-username.github.io`.
- Set a new GitHub Secret with the following key and value:
  - New `PUBLIC_REPO_ACCESS_TOKEN` key and set a value to a GitHub personal access token with the "public_repo" scope.
- Push this project source to your GitHub repository with the following command.
  ```sh
  git branch -m main
  git remote add origin git@github.com:your-github-username/your-github-username.github.io.git
  git push -u origin main
  ```
- Wait until GitHub Actions deployment has finished.
- Go to `GitHub Pages settings` of your repository and set a deployment branch to `gh-pages`. Then click `Save` button.
- Open a browser and navigate to https://your-github-username.github.io.
- You will find your minimal portfolio website in a browser.
- Later, when you edit source code, you just commit your changes and push theme to GitHub again 
  and a project will be deployed to GitHub Pages automatically.
