# Introductory applied machine learning (INFR09029)

# Setting up for DICE

Within this course we will be using Python along with a few open-source libraries (packages). These packages cannot be installed directly, so we will have to create a virtual environment. You can read here if you want to learn about virtual environments, but do not follow any instructions just yet.

Now open a terminal and follow these instructions step-by-step:

* `cd`
* `virtualenv --distribute virtualenvs/iaml_env` (Creates a virtual environment called iaml_env)
* `cd virtualenvs/iaml_env`
* `source ./bin/activate` (Activates the environment, your shell prompt should now change to reflect you are in the iaml_env enviornment)
* `pip install` -U setuptools
* `pip install` -U pip
* `pip install` yolk
* `pip install` numpy
* `pip install` scipy
* `pip install` matplotlib
* `pip install` pandas
* `pip install` statsmodels
* `pip install` scikit-learn
* `pip install` seaborn
* 
You should now have all the required modules installed. Our next step is to make a new directory where we will keep all the lab notebooks, datasets and assignments.

* Open a terminal
* `cd`
* `mkdir iaml_2016`
* `cd iaml_2016`
* 
Now you have two options. We recommend that you directly download a .zip file from https://github.com/agamemnonc/iaml which will contain everything you need and save it in the folder you have just created.

If -and only if- you are familiar and confident with using Git/GitHub you can initiliaze a git directory, add the above repo as remote and pull everything into your local directory. Please use this option only if you really know what you are doing. Unfortunately, we won't be able to provide you with Git/Github support if you run into issues with syncing and using version control in general.

Once you have downloaded the material, you are now ready to start working in the Jupyter environment. First you need to activate the iaml_env environment and start a Jupyter Notebook session from within the folder where the material is stored. Note that you will have to follow this procedure for all labs and assignments.

* `cd`
* `cd virtualenvs/iaml_env`
* `source ./bin/activate` (Activate environment)
* `cd`
* `cd iaml_2016`
* `jupyter notebook`
* Click on `01_Lab_1_Introduction.ipynb` to open it

# Setting up for personal machine (Windows / OS X / Ubuntu)

If you are using a personal machine we recommend that you install an Anaconda distribution (Python version 2.7, choose the appropriate installer according to your operating system).

Once the installation is complete, we need to install the Seaborn package which is the only one not included in the distribution. It's also recommended that you set up a virtual environment for this project. This way, if you update anything in your anaconda base install, this virtual environment will remain unchanged. To create a virtual environment called `iaml`, open a Terminal (or Command Prompt window if you are running Windows) and type:

```bash
conda create -n iaml python=2.7 anaconda seaborn=0.7.0
```

Don't forget to activate the virtual environment every time you begin work from a new terminal:

```bash
source activate iaml
```

Once you have finished installed everything, open a terminal (or Command Prompt in Windows), navigate to the folder where you have downloaded the course material and type:

```bash
jupyter notebook
```

Then click on `01_Lab_1_Introduction.ipynb` to open it.
