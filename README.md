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
