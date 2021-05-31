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
3. Working with fundamental Python libraries:
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
1. You can click on your own binder link in point 12 above, but in this case I will use my own binder link by click the button bellow
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/auliakhalqillah/Introduction-to-Python/main)
 It will direct to new tab window.
2. Wait the building process until you are directed to a Jupyter Notebook workspace automatically. It will takes a few minutes.
3. Now, you are in Jupyter Notebook workspace.
4. If you start from the begining, select **New** > **Python 3** to create a Python file. Otherwise, if you already have a Python file (in Jupyter Notebook format), you can open it and edit it.
5. Let's import a library, such as Numpy by typing

   ```
   import numpy as np
   ```
   
   and click **Run** or press **Shift+Enter**.
6. Type 
   
   ```
   np.linspace(0,2,10)
   ``` 
   and press **Shift+Enter**. It will give a result

   ```
   array([0.        , 0.22222222, 0.44444444, 0.66666667, 0.88888889,
       1.11111111, 1.33333333, 1.55555556, 1.77777778, 2.        ])
   ```
   
 7. Rename the file name e.g. `intropython`.
 8. Unfortunately, you can not save this file into your GitHub repository. The solustion is, you have to download this file by click **File** > **Download as** > **Notebook (.ipynb)**. It will be downloaded automatically.

### 3. Working with fundamental Python libraries
#### a. Numpy
Numpy is a open source library for Python that usefull for numerical computing. Fundamentally, we can generate and modify an array by uisng numpy. For the further operation, we can apply a basic linear algebra, basic statistical operations, shape manipulation and much more ([source](https://numpy.org/doc/stable/user/whatisnumpy.html)). For the begining, I would like to start to generate an array. 
##### 1. arange
First I import a numpy libray by typing

```
import numpy as np
```

where the `np` is as numpy's alias. Next, we can use two methods to generate an array. The first method is by using `np.arange()` and the second method is by using `np.linspace`. So, I start from `np.arange()` method where I generate an array that start from index 0 to index 5th and I assign to `arr` variable by typing as follows command

```
arr = np.arange(0,5)
```

print the result in Jupyter Notebook just type its variable

```
arr
```

it give a result

```
array([0, 1, 2, 3, 4])
```

that means, the 0 is a first index and index 5th is 4. *Note, in Python, the first index is started from 0*
#### b. Pandas
#### c. Matplotlib
#### d. Scipy

   
   
   
   
  

   
   
 


