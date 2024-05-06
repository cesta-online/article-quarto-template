# Anthology Template File for Quarto

## Prerequisites

- Github Account
- Git
- Python 3.6 or later
  > For Mac, use [Homebrew](https://brew.sh/) to install both Git and Python if you don't have them installed already.
- [Quarto](https://quarto.org)
- [VS Code](https://code.visualstudio.com/)
  - GitHub should be configured in VS Code to manage the repository easily
  - Quarto extension can be install in VS Code to preview and render the website

## Usage

- Make a copy of the template to your GitHub account
  - The template can be copied by clicking on the `Use this template` button in the repository
  - Provide a name for the repository and click on `Create repository from template`.
  - The repository name should be in the format `anthology-{project-name}-{session}`. For example, `anthology-knowing-systemic-racism-spring-2023`.
  - Keep the repository public.
  - Copy the repository link to your clipboard.
- Using VS Code, clone the copied repository to your local machine
- Open the cloned repository in VS Code
- Setup the virtual environment using `python -m venv .venv`
- Activate the virtual environment using `source .venv/bin/activate` (Mac & Linux) or `.\.venv\Scripts\Activate` (Windows)
- Install the required packages using `pip install -r requirements.txt`
- Preview the template using `quarto preview`

## Creating a new public github repo for submission

- Run `quarto render` to generate the article web files
- This will create a `public` folder with the website files
- Create a new repository in GitHub website without any files. Use the following naming convention: `anthology-{project-name}-{session}-public`. For example, `anthology-knowing-systemic-racism-spring-2023-public`. This respository link will be used later to push the contents of the `public` folder.
- Create a new directory in your local machine outside the current active repository. This new directory will be used to push the contents of the `public` folder to the new repository in Github.
- Copy the contents of the `public` folder to the new directory
- Open the new directory in VS Code
- Use terminal in VS Code to push the contents to the new repository
  - Initialize the repository using `git init`
  - Set the default branch to `main` using `git checkout -b main`
  - Add the files to the repository using `git add .`
  - Commit the changes using `git commit -m "Initial commit"`
  - Add the remote repository using `git remote add origin <repository-url>`. This repository is the one created in the above step.
  - Push the changes to the remote repository using `git push -u origin main`
- You can also Github Pages to host the website in your Github account and share the link internally for review
- Once your article is finalized, submit the new repository link to publish it in the main website

## Important Notes

- If you are adding a new library to the project, make sure to update the `requirements.txt` file
