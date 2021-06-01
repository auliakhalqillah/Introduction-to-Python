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

where the `np` is as numpy's alias. Next, we can use two methods to generate an array. The first method is by using `np.arange()` and the second method is by using `np.linspace`. So, I start from `np.arange()` method where I generate an array that start from 0 to 5 and I assign to `arr` variable by typing as follows command

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

##### 2. linspace
Now, I'm going to generate an array by using linspace method. The format of np.linspace is np.linspace(start,stop,length of data). First, I generate an array without input a length of data and I assign the result to arr_linspace variable as follows

```
arr_linspace = np.linspace(0,0.5)
arr_linspace
```
```
len(arr_linspace)
```
and the result

```
array([0.        , 0.01020408, 0.02040816, 0.03061224, 0.04081633,
       0.05102041, 0.06122449, 0.07142857, 0.08163265, 0.09183673,
       0.10204082, 0.1122449 , 0.12244898, 0.13265306, 0.14285714,
       0.15306122, 0.16326531, 0.17346939, 0.18367347, 0.19387755,
       0.20408163, 0.21428571, 0.2244898 , 0.23469388, 0.24489796,
       0.25510204, 0.26530612, 0.2755102 , 0.28571429, 0.29591837,
       0.30612245, 0.31632653, 0.32653061, 0.33673469, 0.34693878,
       0.35714286, 0.36734694, 0.37755102, 0.3877551 , 0.39795918,
       0.40816327, 0.41836735, 0.42857143, 0.43877551, 0.44897959,
       0.45918367, 0.46938776, 0.47959184, 0.48979592, 0.5       ])
```

as we can see, the array has been generated start from 0 to 0.5 in 50 length of data as default configuration. Next, I generate an array with input a length of data e.g. 70 values and I assign the result to arr_linspace_length variable as follows

```
arr_linspace_length = np.linspace(0,0.5,70)
arr_linspace_length
```

and the result

```
array([0.        , 0.00724638, 0.01449275, 0.02173913, 0.02898551,
       0.03623188, 0.04347826, 0.05072464, 0.05797101, 0.06521739,
       0.07246377, 0.07971014, 0.08695652, 0.0942029 , 0.10144928,
       0.10869565, 0.11594203, 0.12318841, 0.13043478, 0.13768116,
       0.14492754, 0.15217391, 0.15942029, 0.16666667, 0.17391304,
       0.18115942, 0.1884058 , 0.19565217, 0.20289855, 0.21014493,
       0.2173913 , 0.22463768, 0.23188406, 0.23913043, 0.24637681,
       0.25362319, 0.26086957, 0.26811594, 0.27536232, 0.2826087 ,
       0.28985507, 0.29710145, 0.30434783, 0.3115942 , 0.31884058,
       0.32608696, 0.33333333, 0.34057971, 0.34782609, 0.35507246,
       0.36231884, 0.36956522, 0.37681159, 0.38405797, 0.39130435,
       0.39855072, 0.4057971 , 0.41304348, 0.42028986, 0.42753623,
       0.43478261, 0.44202899, 0.44927536, 0.45652174, 0.46376812,
       0.47101449, 0.47826087, 0.48550725, 0.49275362, 0.5       ])
```


#### b. Pandas
#### c. Matplotlib
#### d. Scipy

   
   
   
   
  

   
   
 


