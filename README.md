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
- Running `quarto preview` will create the website files in the `public` folder. You can use Github Pages to host the website in your Github account and share the link internally for review. The website link will be in the format `https://{github-username}.github.io/{repository-name}/public`.

## Creating a new public github repo for submission

- Once your article is ready for submission, write an email to `cesta-online@stanford.edu` with the following information:
  - Subject: Anthology Submission: {Project Name}
  - Body:
    - Your article link hosted in Github Pages
    - Your Github Username
- The CESTA team will review your submission. If approved, an empty repository will be created in the CESTA Github organization and you will be added as a collaborator.
- Run `quarto render` to generate the article web files in the `public` folder of your current repository.
- You can then **push your article files inside the `public` folder of your current repository** to the new repository provided by CESTA.
- Once the files are pushed to the new repository, the CESTA team will review the submission and publish the article on the CESTA website.

## Important Notes

- If you are adding a new library to the project, make sure to update the `requirements.txt` file
