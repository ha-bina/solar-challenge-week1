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
%pip install pandas
import pandas as pd
#Summary Statistics & Missing-Value Report
df = pd.read_csv("togo-dapaong_qc.csv")  
df.describe()
missing = df.isna().sum()
missing[missing > 0]
# Columns with >5% missing
threshold = 0.05 * len(df)
missing[missing > threshold]