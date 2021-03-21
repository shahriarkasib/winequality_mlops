1. At first create a project and a new conda environment
   if using command prompt use the code below:
   conda create -n <env_name> 
   

2. create a requirements.txt file which will have all the packages to be installed.
Use the following command to install all the dependencies:
   pip install -r requirements.txt
   

3. Create a template.py to create different directories and files needed.

4. keep the template.py to .gitignore file so that it does not go to git (optional)

5. create a directory named data_given to keep the data we will work with.

6. keep your data to data_given folder

7. Run the following commands afterward one by one:

```bash
  git init
```
```bash
  dvc init
```

```bash
dvc add <datasource path>
```
```bash
  git add .
```
```bash
  git commit -m "message"
```
```bash
  git branch -M main
```
```bash
  git remote add origin <repositiory url>
```

```bash
  git push -u origin main
```

One line code for changes and git push

```bash
git add . && git commit -m "give the message here" && git push -u origin main
```

8. write the params.yaml file
9. create get_data.py
10. create load_data.py
11. write stage load_data in dvc.yaml
12. run the following command
```bash
   dvc repo
```
13. create split_data.py
14. Again do 11 for spit_data stage
15. Run 12 again
16. create train_and_evaluate.py to train and evaluate model
17. Create a folder named report
18. create a json file named params.json which will keep trcak of the model parameters
19.create a json file named scores.json which will keep trcak of the model scores
    20. dvc metrics show to show the scores and parameters
   21. dvc metrics diff to show the difference in scores after changing parameters