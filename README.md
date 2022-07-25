# mckl-workshop

### This repo is for the MCKL workshop using git and docker.

# mckl-workshop

### This repo is for the MCKL workshop using git and docker.

### Round 1 SETUP
**Everyone in the team**
> 1. Pull this repo and checkout your team's branch
```
git checkout <branch_name>

TO VIEW WHAT BRANCH YOU'RE AT
git branch
```

**Someone in the team**
> 2. Copy the files from the chosen programming language into your team's folder
> 3. Change directory into your team folder
> 4. Add the files into the git branch
> 5. Commit and push the changes to your team's branch

**Everyone in the team**
> 6. Pull the changes made by the appointed teammate.
> 7. In your team's directory test docker build and run.
```
docker build .

TO VIEW IMAGES BUILT
docker image ls 

TO RUN DOCKER IMAGE
docker run <container id>
```

> 8. From your team's branch checkout to another new branch so that when you're working on your own task it will not affect your teammates
```
git checkout -b <new_branch_name>
```

###  Round 2
**Application**
> 1. Update application code to take in some user input which is a number and print the input out. Program ends/exit once the output is printed. (input will only be a single string with no spaces)

**Startup Script**
> 2. Modify _entrypoint.sh_ script to run your group application (Just on your local computer will do).
Note down what steps you took to run the script on your local computer.
i.e. When you run the script "entrypoint.sh" it will run "app.py" on your computer.
Note : If your teams chosen programming language requires compilation of codes. Entrypoint.sh script should include the command to compile and run. 

**Dockerfile**
> 3. Ensure that When the container builds ensure that _entrypoint.sh_ will be in the same directory as your team's application code. (proof / verify that it works)
> 4. When commands below are run, hello world and the bash echo will both be displayed (which runs first does not matter)
```
docker build .
docker run <container id>
```

### Final Round

**As a team**
> 1. Using git, combine all your work together into a single branch. (your team's branch will do)

> 2. Combine your work in Round 2 so when the instructor/another team does a 
```
dockerbuild . 
docker run <container id>
```
It will run as expected.


Reminder : This is __**NOT**__ a programming workshop. Use whatever way to complete the challenges as long it works.

### Basic Helpful commands 
```
UBUNTU / LINUX

SHOW CURRENT DIRECTORY 
pwd

LIST FILES IN CURRENT DIRECTORY 
ls

CHANGE DIRECTORY 
cd <diretory name>

CHANGE DIRECTORY (BACK / UP ONE LEVEL)
cd ..


GIT 

TO VIEW WHAT BRANCH YOU'RE AT
git branch

CHANGE TO ANOTHER BRANCH
git checkout <branch name>

SAVE ALL YOUR CHANGES 
git commit -am "enter your message here"

PUSH YOUR CHANGES TO GITHUB
git push


DOCKER 

LIST CONTAINERS BUILT
docker image ls

DOCKER BUILD (requires Dockerfile to be present)
docker build .

RUN CONTAINER BUILT
docker run <container id>
```