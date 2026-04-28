# NC-TaxTriggers
Data and code for article, "Adjusting North Carolina Tax Triggers Makes Good Economic Sense".

## How to replicate the analyses

### Install Python
The code for these analyses is written in the Python programming language. You must have Python installed on your computer to run the code. I recommend installing the Anaconda distribution of Python. You can install this for Mac, Windows, and Linux machines by going to https://www.anaconda.com/download. I recommend clicking "Skip registration" to go straight to downloading the free Python distribution. Just follow the instructions.

### Fork and clone or download the repository
The code, data, and images in this analysis are stored in the GitHub repository https://github.com/OpenSourceEcon/NC-TaxTriggers. You can either download the files to your machine, or you can use the Git version control software function of forking and cloning the repository. I recommend the Git approach of forking and cloning the repository.
- If you choose to download the files without using Git software, to to the https://github.com/OpenSourceEcon/NC-TaxTriggers GitHub repository page in your browser, press the green "Code" button, and select "Download ZIP".
- If you choose to use Git version control software and fork and clone the repository:
    - Make sure Git software is installed on your computer. In your Terminal on a Mac or Linux machine or in the Command Prompt on a Windows machine, type `git --version`. If Git software is installed, a version number will show in the output (e.g., `git version 2.53.0`).
    - If Git is not installed on your computer, install Git using the method below that corresponds to your operating system. Good instructions are at https://git-scm.com/install/.
        - For Mac:
            - In your Terminal, type the following command to install the Homebrew package manager: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
            - Use Homebrew package manager to install Git software. In your Terminal, type the following command: `brew install git`
            - To make sure Git is correctly installed, type the following command in your Terminal: `git --version`. It should tell you which version of the Git version control software you have (e.g., `git version 2.53.0`).
        - For Linux, follow instructions at https://git-scm.com/install/linux.
        - For Windows, following instructions at https://git-scm.com/install/windows.
    - Fork the repository to your GitHub account. This is done by going to the home page of the main repository https://github.com/OpenSourceEcon/NC-TaxTriggers, clicking the "Fork" button in the upper-right, choosing your account as the "Owner", and clicking the green "Create fork" button. This will create an exact copy of the repository in your GitHub account. For example, my clone of the main repository is at the URL https://github.com/rickecon/NC-TaxTriggers.
    - Clone the repository from your GitHub account to your hard drive. In your Terminal (Mac/Linux) or Command Prompt or Anaconda Prompt (Windows), navigate to the folder where you want the `NC-TaxTriggers` repository to reside. Type the following command in your Terminal: `git clone https://github.com/[YourGitHubHandle]/NC-TaxTriggers.git`, where the `[YourGitHubHandle]` portion is your GitHub handle. For example, mine is `rickecon`. Now you have an exact copy of the main repository on your GitHub account in the cloud and on your hard drive.

### Create a virtual environment
This repository of Python code is set up to use Python's `uv` package to create a virtual environment that has all the Python packages necessary to run these analyses. And the resulting `uv.lock` will create a virtual environment that will exactly replicate the results across operating systems. To create the virtual environment from the `uv.lock` file, navigate to the repository directory `NC-TaxTriggers` in your Terminal (Mac/Linux) or Anaconda Prompt (Windows). Type `uv sync`. Then activate the resulting virtual environment by typing `source .venv/bin/activate`.
