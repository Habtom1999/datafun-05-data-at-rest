# datafun-05-data-at-rest
# Files,Exceptions, and SQL Data Structure
---
Jupyter Notebooks are a popular way to create and share documents for data analytics. They are interactive, easy to share, and support a wide variety of data science tools.

In this module, you'll read from data files, process the data, and write to output files. We'll also look at using Python to work with light-weight, file-based relational database SQLite using the sqlite3 module from the Python Standard Library.

This module deals with data at rest. Data at rest may be kept in:

files,
relational databases (e.g., SQLite, SQL Server, Oracle),
NoSQL datastores (e.g., MongoDB)
Graph databases (e.g., Neo4J)
and more.
We'll look at how to read and write from files and relational databases.

Data at rest is only part of the story. In analytics, there is also data in motion. Data in motion is unbounded - infinite - and is covered in our program course on Streaming Data.

Step 1: GET STARTED
Log in to your GitHub account.machine.Open a terminal in VS Code. Use the menu View / Terminal. In Windows, use PowerShell, in Mac, use bash. Verify you've added some essential packages to your default Python environment.

Step 2: Create a new GitHub repo named datafun-05-data-at-rest. Follow conventions - use kebob, lower case, no spaces.

Srep 3: Git clone your new repo into your Documents folder.

Add .gitignore
Added gitignore
The .gitignore file tells Git files to ignore when committing changes.
Review the gitignore file, you can use it without modification.
Modify README.md
Learn to edit and customize README.md files, which provide a quick overview of the project and instructions for running it.
Scan requirements.txt
The requirements.txt file lists the packages used in the project.
You may not use all them and may want to add others. Modify this list as you like.
🚀 Rocket Tip: When employers ask for years of experience with a language, it's not the syntax - that's learned in a few days. It's the experience with the tools, libraries, and frameworks that takes time.

Step 4: Set up a Virtual Enviroment
Next, we'll create and activate a virtual environment specifically for this project. We'll also install additional packages required for this project.

Create a Virtual Environment
Open the terminal in VS Code. (View / Terminal)
Run the following command to create a virtual environment for this project.
python -m venv .venv
Verify that a new .venv folder was created. It may take a while for the command to complete.

🚀 Rocket Tip: When VS Code Python Extension offers to select the Environment, say Yes.

Activate the Virtual Environment
Wait for the creation to finish, then activate the virtual environment:

For PowerShell: .venv\Scripts\Activate
For macOS/Linux: source .venv/bin/
🚀 Rocket Tip: Notice the terminal changes to reflect the active virtual environment.

Install Dependencies to the Active Virtual Environment
Install additional project dependencies into the active virtual environment. The packages ipykernel and jupyterlab are required to run a notebook. The packages pandas, matplotlib, and seaborn are used to work with data and charts.

python -m pip install --upgrade pip ipykernel jupyterlab
python -m pip install --upgrade pandas matplotlib seaborn
python -m pip install --upgrade voila
Alternatively, you can install all the packages listed in the requirements.txt file.

python -m pip install --upgrade -r requirements.txt
Note: The --upgrade parameter gets the lastest version of each package.

Step 5: Working with Notebooks
In the active virtual environment, create a Python kernel to run our notebooks.

python -m ipykernel install --user --name .venv --display-name "Python (.venv)"
Execute an existing notebook
Create a new notebook
In VS Code, from the menu, select View / Command Palette. Type notebook and select Jupyter: Create New Blank Notebook. This will create a new notebook in the project folder. Save the notebook with a name like yourname-notebook.ipynb.
