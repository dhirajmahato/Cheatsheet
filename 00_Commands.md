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
10. ls(ubuntu/macOS) , dir (windows)
11. pip install cookeiecutter-data-science  # for project structure
12. git identity
    ```
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```
13. github SSH connection
    ```
    Generate an SSH Key:
    ssh-keygen -t ed25519 -C "dhiraj.mahato.iitbhu@gmail.com"
    Add Your SSH Key to the SSH Agent:
    eval "$(ssh-agent -s)"
    ssh-add ~/.ssh/id_ed25519
    Add the SSH Key to Your GitHub Account:
    cat ~/.ssh/id_ed25519.pub # copy from here and add a new ssh key in github account
    ```
14. github push cmds for local repo
    ```
    git init
    git add .
    git commit -m "first commit"
    git remote add origin git@github.com:dhirajmahato/Music_ml.git
    git branch -M main
    git push -u origin main
    ```
 15. git status
 16. git remote set-url origin git@github.com:your-username/your-repository.git   #update remote url
 17. git remote remove origin


