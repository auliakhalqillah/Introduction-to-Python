# Introduction to Python
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/auliakhalqillah/Introduction-to-Python/main)

## Introduction
I create this repository to share about fundamental of Python programming language based on my experience. Python has been introduced by [Guido van Rossum](https://en.wikipedia.org/wiki/Guido_van_Rossum) in 1991. Currently, Python is a one of common programming languages that widely used in this century because the language is close to human language and easy to be learned. This programming language can be applied in some fields, such as:

- Web and Internet Davelopment
- Scientific Numeric
- Education
- Desktop GUIs
- Software Davelopment
- Bussiness Applications
- and much more

Python can be installed in Linux, Windows and Mac OS, for more information about the installation, you can visit the [Python's website](https://www.python.org/downloads/).

In this repository, I would like to explain:

1. How to setup Python online by using [mybinder.org](https://mybinder.org/) and Github Repository
2. Working with Jupyter Notebook
3. Working with fundamental libraries:
   - [Numpy](https://numpy.org/)
   - [Pandas](https://pandas.pydata.org/)
   - [Matplotlib](https://matplotlib.org/)
   - [Scipy](https://www.scipy.org/)

I hope this repository may help all of you to learn about Python programming language. Enjoy it :coffee:

## Content
### 1. How to setup Python online by using mybinder.org and Github Repository

1. You have to create a [Github](https://github.com/) account. If you already have, just ignore this step. Go to the next step.
2. Log in to your Github.
3. Create a new repository. Set a repository name e.g. `Introduction to Python`. Don't forget to create a README.md file by checking a check box.
4. Add new file of environment file by click on **Add files** > **Create new file**. Set the file name as **environment.yml**. The environment.yml is a list of dependencies that to be used in your Python online. For example, the content of environment.yml file are:
   ```
   name: python36-environment
   dependencies:
      - python=3.6
      - numpy
      - pandas
      - matplotlib
   ```
   that means, in your Python online system will be installed all dependencies according to your environment file. Note, you can change the name in environment file.
5. Create a folder in your computer. Give it a folder name e.g. **test**. The **test** folder contain two files, there are **test.ipynb** (Jupyter Notebook empyt file) and **test.md** (Markdown empty file).
6. Click **Add File** > select **Upload Files**. Then, choice/drag a file/folder that want to be uploaded. For example, I upload a **test** folder that I create previously. Click **Commit changes** after all files/folders are complete uploaded.
7. Go to the [mybinder.org](https://mybinder.org/). It will open a new tab window.
8. Copy the previously repository link e.g. `https://github.com/<your-user-name->/Introduction-to-Python` that has been created and paste to mybinder.
9. Type in a Get ref as master or main.
10. Click **Lunch** button and wait the process.
11. When the process of lunch is complete, the page will refresh automatically and direct you to Jupyter Notbeook workspace.
12. To access your Python online, you should copy a link from mybinder, for example format
   ```
   [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/<user-name>/Introduction-to-Python/main)
   ```
   and paste it to your README.md file in your repository just you create. (*user-name is your GitHub user name*).
 
 13. Now you are in Jupyter Notebook workspace. You will see the **test** folder. Click this folder and you will see the **test.ipynb** and **test.md** file. Click on **test.ipynb** file and you will be directed to a Jupyter Notebook project file. Now, you can write your Python code.

### 2. Working with Jupyter Notebook
1. You can click on your binder link in point 12 above, but in this case I will use my own binder link by click [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/auliakhalqillah/Introduction-to-Python/main). It will direct to new tab window.

   
   
   
   
  

   
   
 


