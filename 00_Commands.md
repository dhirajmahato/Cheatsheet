# commands
1. cls -- Clean the screen
2. pwd
3. cd, cd ..
4. rm -rf filename
5. py --version
6. python --version
7. brew update python3
8. brew upgrade pyhton3
9. pip --version   // >python -m pip install --user --upgrade pip// pip install virtualenv // python -m venv env
10. python.exe -m pip install --upgrade pip
11. ls(ubuntu/macOS) , dir (windows)
12. pip install cookeiecutter-data-science  # for project structure
13. git identity
    ```
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```
14. github SSH connection
    ```
    Generate an SSH Key:
    ssh-keygen -t ed25519 -C "dhiraj.mahato.iitbhu@gmail.com"
    Add Your SSH Key to the SSH Agent:
    eval "$(ssh-agent -s)"
    ssh-add ~/.ssh/id_ed25519
    Add the SSH Key to Your GitHub Account:
    cat ~/.ssh/id_ed25519.pub # copy from here and add a new ssh key in github account
    ```
15. github push cmds for local repo
    ```
    git init
    git add .
    git commit -m "first commit"
    git remote add origin git@github.com:dhirajmahato/Music_ml.git
    git branch -M main
    git push -u origin main
    ```
 16. git status
 17. git remote set-url origin git@github.com:your-username/your-repository.git   #update remote url
 18. git remote remove origin
 19. Within Jupyter:  !pip install package_name
 20. Python system location: where python, where pip   --> multiple Python environments or installations are present on your system, and each has its own associated pip.
 21. pip list, pip list --user
 22. python -m site         // for site_pakage 

