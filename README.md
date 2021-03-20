1. At first create a project and a new conda environment
   if using command prompt use the code below:
   conda create -n <env_name> 
   

2. create a requirements.txt file which will have all the packages to be installed.
Use the following command to install all the dependencies:
   pip install -r requirements.txt
   

3. Create a template.py to create different directories and files needed.

4. keep the template.py to .gitignore file so that it does not go to git (optional)

5. create a directry named data_given to keep the data we will work with.

6. keep your data to data_given folder

7. Run the following commands afterward:
   
   - git init
   - dvc init
   - dvc add data_given\winequality.csv
   - git add .
   - git commit -m "message"
   