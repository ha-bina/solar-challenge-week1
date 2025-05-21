# solar-challenge-week1
# configure user name and email
git config --global user.name 'Habtam'
git config --global user.email 'habtam440@gmail.com'
# To access the repository from github and clone 
git clone http://github.com/ha-bina/solar-challenge-week1.git
cd solar-challenge-week1
# Create and activate phython environment
git venv .venv
.venv/scripts/activate
# prepare and install requirements
pip freeze > requirements.txt
pip install -r requirements.txt
# create a branch
git checkout -b setup-task
# Create a git ignore
touch .gitignore
git commit -m "remove tracked file and updat .gitignore"
git rm --catched temp
git rm --temp
vim gitignore