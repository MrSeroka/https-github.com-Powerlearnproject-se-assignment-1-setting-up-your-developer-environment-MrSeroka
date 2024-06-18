# https-github.com-Powerlearnproject-se-assignment-1-setting-up-your-developer-environment-MrSeroka


# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   
Check System Requirements
For Windows, check system requirements first before installing. Open Start Menu and type System Requirements, then Enter to view System Information. My Pc runs on x64-bit.


Backup Data
Before installing, backup data to prevent data loss during installation process.
By signing into OneDrive account used by Microsoft account, drag and drop files into OneDrive folder in File Explorer or alternatively use OneDrive App to upload files.

Download Windows 11
Visit the official Microsoft website https://www.microsoft.com/software-download/windows11 and download the Windows 11 installation file.
1. Click Download Now under Windows 11 Installation Assistant, run the Installation Assistant. 

![alt text](<Screenshot 2024-06-18 200149.png>)

2. Open the downloaded file under downloads
3. Follow the On-Screen intructions. The Installation Assistant will check if your PC meets the minimum hardware requirements and if your PC is compatible and if so, Installation Assistant will download and install.
4. After the Installation is complete, the Assistant will ask you to restart your computer and finalized the installation process while upgrading it.
5. After restarting, complete the set up instructions of Windows 11 by selecting your region, keyboard layout and signing in your Microsoft Account.
6. Final step is to check for Updates by going to Setting > Windows Update and check if your system is up-to-date.

Restore your backed-up data and install any necessary applications.
By following these steps, you can successfully download and install Windows 11 on your PC.

2. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download

1. Go to  https://code.visualstudio.com/Download
 click Windows Download link to download Visual Studio Code(VS Code)
Check your system requirements before downloading, mine is x64 bit.
 Open Start Menu and type System Requirements, then Enter to view System Information.
![alt text](<Screenshot 2024-06-18 200439-1.png>)
![alt text](<Screenshot Git confiq --global-2.png>)

2. Once downloaded, click downloaded files and and double click on it to start the installation process 

3. Follow the on-screen instructions in the setup wizard, click next to accept the license agreement then next choose the installation location.
Create a desktop icon and adding VS Code to the PATH. Click Next to finish  Installing.

4. Launch VS Code and run as administrator. Run a terminal and install Extentions (Ctrl+Shift+X) such as Python.

5. Open setting on the gear icon and adjust settings according to your preference.

3. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com

To download Git Installer, go to git-scm.com and download the latest version for Windows. The latest source release: 2.45.2

During Installation you can adjust default settings based on your needs but they are normally fine. Choose Git from the command line  and from 3rd party software to adjust your PATH environment. Use the bundled OpenSSh then complete the installation and click Finish.

Configure Git after installation by opening Git Bash from your Start Menu, search Git Bash then left click to Run Administrator.
Open a new Terminal and type git config to setup your username. git config --global username(Your Name) and git config --global user.email (email@youremail.com)

![alt text](<Screenshot Git confiq --global-1.png>)

Verify Configuration by entering git config --list

 Creating  a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit

1. Visit [GitHub website](https://github.com/) and login into your GitHub account.
2. Oen a New Repository by clicking the + icon in the upper-right corner and select New repository.Enter a name for your Repository and a brief description(optional) for your repository. The next step is to choose whether it will be a Private/Public repository. After you open a README file

3. Clone the Repository by clicking the <> Code icon, under HTTPS tap copy the url. Then open Git Bash and right click to run as administrator, open a new terminal and type a command: git clone repository -(past url you copied), a copy will be created on your computer
![alt text](<Screenshot 2024-06-18 200804.png>)

4. Add files to the repository directory, commit them and push to GitHub:
git init
git add .
git commit -m "Initial commit"
git remote add origin (past your copied repository url)
git push -u origin main

4. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.

To download and install Python on your computer. Visit http://wwww.python.org and download the latest version of Python for your operating system. The Latest Python is 3.12.4
![alt text](<Screenshot 2024-06-18 200928.png>)

After completing the download, run the installer and follow the installation wizard.

Right click on the Python file and Add Python to PATH then click on customize Installation. Ensure that these options are checked: 
- Documentation
- pip
- tcl/tk and IDLE
- Python test suite
- py launcher
- install for all users

Under Advanced Options:
- Create shortcuts for installed applications
- Add Python to environment variables
- Precompile standard library
- Click Install.
 
 On the Start Menu search for Command Prompt and command python --version.
 It will display the installed versiom of Python
 Command pip --version to display pip version installed


5. Install Package Managers:
   If applicable, install package managers like pip (Python).

After successfully installing Python and Adding Python to PATH you neec to verify installation.
On the Start Menu, search Command Prompt and type the command python --version  it will display the Python version installed 
To ensure pip is Installed, which is usually included in Python Installations. 
Type command pip --version  it will show pip installation status and if not installed type python -m ensurepip --upgrade  to install pip manually

6. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html

Visit https://dev.mysql.com/downloads/windows/installer/5.7.html and select appropriate opersting system then download. My PC runs on x64 bit

Open the downloaded file to run installation and choose Developer Default and follow the installatiom promts

During Installation prompt configure MySQL serve set config type to Developer Machine, Port Number is 3306, set Root Password and create a User.

After Installation the MySQL Installer will give you the option to start the MySQL Server after the installation.

To verify Installation Open Command Prompt and run command to log in to MySQL as the root user: mysql -u root -p
Enter Root Password set during installation.

7. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.

Docker is a popular virtualization tool used to create and manage containers for isolating project dependencies. 

Create a Dockerfile by creating a file named Dockerfile in your project directory to define the container's configuration.
Use commands like FROM, RUN, COPY, and CMD to specify the base image, install dependencies, copy project files and set the default command.

Build the Docker Image by running the command 
docker build -t image_name . in the project directory to build the Docker image based on the Dockerfile.

Run the Docker Container by using the comman
docker run -it --name container_name image_name to start a container based on the built image.

Virtual machines (VMs) can also be used to ensure consistent environments across different machines.

To setup a Virtual Machine you neec to choose a Virtualization Software such as VirtualBox, VMware, or Hyper-V.


Download and install the chosen virtualization software on your machine then open the virtualization software and create a new virtual machine by specify the operating system, memory, storage, and other settings for the virtual machine.

Install the necessary dependencies and tools within the virtual machine to mirror the project's environment then take a snapshot of the virtual machine or export it as an appliance to create a reusable template for consistent environments.

8. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.

Syntax highlighting improves code readability by displaying text in different colors based on its role in the programming language.

With Visual Studio Code when can use extentions such as:
- Python. A Built-in support with the Python extension.
- JavaScript/TypeScript. A Built-in support with the VSCode extensions for JavaScript and TypeScript.
- C++. C/C++ is an extension by Microsoft.

Linters analyze code to flag programming errors, bugs, stylistic errors and suspicious constructs.

Visual Studio Code:
- ESLint used for JavaScript and TypeScript linting.
- Pylint used fot Python linting.
- TSLint used for TypeScript linting.
- Flake8 is another popular linter for Python.

Code formatters automatically arrange code according to a specified style guide.

Visual Studio Code:
- Prettier is a popular code formatter for JavaScript, TypeScript, CSS, and more.
- Black is a formatter for Python.
- clang-format is For C++.

Version control extensions integrate tools like Git into the editor for managing code repositories.

Visual Studio Code:
- GitLens enhances the built-in Git capabilities with additional features.
- Git History gives us a view for Git history and diffs.

Installing Instructions for Extentions for Visual Studio Code
1. Open VSCode.
2. Go to the Extensions view by clicking the Extensions icon in the Activity Bar on the side of the window or by pressing Ctrl+Shift+X.
3. Search for the desired extension. It must show a tick to show it is approved and trusted.
4. Click Install.
