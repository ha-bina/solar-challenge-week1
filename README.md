# solar-challenge-week1
git config --global user.name 'Habtam'
git config --global user.email 'habtam440@gmail.com'
git clone http://github.com/ha-bina/solar-challenge-week1.git
cd solar-challenge-week1
.venv/scripts/activate

pip freeze > requirements.txt
pip install -r requirements.txt
git checkout -b setup-task
touch gitignore
git commit -m "remove tracked file and updat .gitignore"
git rm --catched temp
git rm --temp
vim gitignore