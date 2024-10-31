# mainmodule
**Executes hello world from Submodule repository**

## Instructions

**1 - Cloning the repository**

git clone https://github.com/PedroBatista1/mainmodule.git

**2 - Initialize submodules**

(fetches source code from the submodule repository in https://github.com/PedroBatista1/submodule)

a. git submodule init

b. git submodule update

**3 - Create a feature branch, apply a change and create a PR to trigger the build through the github action in .github/workflow.**

a. git checkout -b feature/new_branch 

b. Apply any change to a file

c. git add file

d. git commit -m "A change"

e. git push -u origin feature/new_branch

d. Create a Pull Request in GitHub

Through this process the github action will be invoked, and the makefile in the repository is used to build the program in the Ubuntu GitHub remote machine (other OS can be chosen).
