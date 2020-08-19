---
title: "Save pandas dataframe to spreadsheet in google colabratory"
date: 2020-07-16T22:05:50+09:00
draft: false
---

# Intro
The method to save a pandas dataframe to a google spread sheet like `pd.to_csv()`.

# How to use df2gspread
First, we have to install [df2spread](https://pypi.org/project/df2gspread/) and mount your drive.

```
!pip install df2gspread
```
```
from google.colab import drive
drive.mount('/gdrive')
```
(or click left side button in google colab)

## Example
```py
from oauth2client.client import GoogleCredentials
from df2gspread import df2gspread as d2g

df = pd.DataFrame({'col':[1,2,3,4,5]})

d2g.upload(
    df,
    'SPREADSHEET_PATH',
    'WORKSHEET_NAME',
    credentials=GoogleCredentials.get_application_default()
)
```
If the directory `'SPREADSHEET_PATH'` dose not exist, `d2g.upload` create the path. If exist, they overwrite the file.