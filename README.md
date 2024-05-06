# Anthology Template File for Quarto

## Prerequisites

- Git
- Python 3.6 or later
  > For Mac, use Homebrew to install both Git and Python if you don't have them installed already.
- [Quarto](https://quarto.org)
- [VS Code](https://code.visualstudio.com/)
  - GitHub should be configured in VS Code to manage the repository easily
  - Quarto extension can be install in VS Code to preview and render the website (Optional)

## Usage

- Make a copy of the template to your GitHub account
- Using VS Code, clone the copied repository to your local machine
- Open the cloned repository in VS Code
- Setup the virtual environment using `python -m venv .venv`
- Activate the virtual environment using `source .venv/bin/activate` (Mac & Linux) or `.\.venv\Scripts\Activate` (Windows)
- Install the required packages using `pip install -r requirements.txt`
- Preview the template using `quarto preview`
- Render the updated website using `quarto render`

## Creating a public github repo for submission

- Run `quarto render` to generate the website
- This will create a `public` folder with the website files
- Create a new repository in GitHub without any files. Use the following naming convention: `anthology-{project-name}-{session}`. For example, `anthology-knowing-systemic-racism-spring-2023`. This respository link will be used later to push the contents of the `public` folder.
- Create a new directory in your local machine outside the current repository. This will be used to push the contents of the `public` folder to the new repository.
- Copy the contents of the `public` folder to the new directory
- Open the new directory in VS Code
- Initialize the repository using `git init`
- Set the default branch to `main` using `git checkout -b main`
- Add the files to the repository using `git add .`
- Commit the changes using `git commit -m "Initial commit"`
- Add the remote repository using `git remote add origin <repository-url>`. This repository is the one created in the above step.
- Push the changes to the remote repository using `git push -u origin main`
- You can also Github Pages to host the website in your Github account and share the link internally for review
- Once your article is finalized, submit the new repository link to publish it in the main website
