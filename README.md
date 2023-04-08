# Ex03-Univariate-Analysis 

## Aim:

To read the given data and perform the univariate analysis with different types of plots.

## Explanation:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm:

### Step1:

Read the given data.

### Step2:

Get the information about the data.

### Step3:

Remove the null values from the data.

### Step4:

Mention the datatypes from the data.

### Step5:

Count the values from the data.

### Step6:

Do plots like boxplots,countplot,distribution plot,histogram plot.

## Program:

DEVELOPED BY : YOGESH B

REGISTER NO : 212221220062
```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
## Output:

## Dataset:

![image](https://user-images.githubusercontent.com/129483978/229035180-1ca26200-ff18-4a40-9918-d96e72e8117a.png)

## Head:
![image](https://user-images.githubusercontent.com/129483978/229035348-3fdaec29-da4f-4bcf-bbcb-274f42be51ad.png)

## Info:
![image](https://user-images.githubusercontent.com/129483978/229035471-6c5e57fb-df1f-4bd5-964c-4580e514aa26.png)

## Describe:

![image](https://user-images.githubusercontent.com/129483978/229035532-37d0e876-dd79-4f84-beab-146cb69c1211.png)

## Isnull:

![image](https://user-images.githubusercontent.com/129483978/229035733-510e524a-1b3d-4a23-894b-2465981b3a68.png)

## dtypes:

![image](https://user-images.githubusercontent.com/129483978/229035814-1adff3b5-a97e-4006-98c7-2c0ab0abd4ad.png)

## Valuecount:

![image](https://user-images.githubusercontent.com/129483978/229035930-c9105f35-963a-4d10-83fc-bafb7f33ca0a.png)

## Boxplot:

![image](https://user-images.githubusercontent.com/129483978/229036036-340bcdf4-3c1b-45bc-ab1c-619f0412d1e4.png)

## Countplot:

![image](https://user-images.githubusercontent.com/129483978/229036129-dfebf51c-3e78-46ee-8f4c-24e126d10413.png)

## Distribution plot:

![image](https://user-images.githubusercontent.com/129483978/229036203-81ec5dd2-180f-4483-84d8-84c8cf621c53.png)

## Histogram plot:

![image](https://user-images.githubusercontent.com/129483978/229036298-fe2d415f-12e1-48e0-9ffc-6d5cf250e6f9.png)

## Result:

Thus we have read the given data and performed the univariate analysis with different types of plots.







