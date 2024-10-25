# Numpy

```python
import numpy as np
```


l1=[1,2,3]
myarr=np.array(l1)

myarr=np.array(l1,dtype=float)
myarr

print("my array size is",myarr.size)
print("my array type is ",myarr.dtype)
print("my array deminision is ",myarr.ndim)
print("my array shape is ",myarr.shape)

myarr=np.identity(3)
myarr

print("my array deminision is ",myarr.ndim)
print("my array shape is ",myarr.shape)

np.arange(1,101)

np.random.random(size=3) # 0-1

np.random.randint(1,7,size=1)

### Boolean_indexing

np.random.seed(7)
arr=np.random.randint(30,size=10)

arr

arr>10

arr[arr>10]

np.where(arr>10)

arr[(arr>20) & (arr<30)]

arr[np.where((arr>20) & (arr<30))]

### copy, delete, append, insert,sort & flip method

b=np.copy(arr)

b

np.delete(b,[1,2])

np.append(b,[10,11,12])

np.insert(b,4,[33])

np.flip(np.sort(b))

### identity & zero matrix

np.identity(5)

np.eye(5)

np.zeros((5,5))

### Reshape


l1=[1,2,3]
l2=[4,5,6]


arr=np.array([l1,l2])

arr.shape

arr

arr.reshape(3,2,order="C") # F is for column and C is rows

ls=[[1, 2, 3],[4, 5, 6]]

ls[:]

arr

arr[1,1:3]

### Transpose

np.transpose(arr)


arr.T

# pandas Series

import pandas as pd
import numpy as np

pd.Series()

pd.Series(['A','B','C'],index=np.arange(1,4))

dic={1:'A',2:'B',3:'C'}
ser=pd.Series(dic)

ser.sort_values(ascending=False)

ser.sort_index()

dic={'a1':36,'a2':13,'a3':30,'a4':36,'a5':46}
ser=pd.Series(dic)

ser.mean()

ser.sum()

ser.between(30,40)

ser.drop('a5',inplace=True)

ser

## Pandas DataFrame

import pandas as pd

df=pd.DataFrame()

ser_dict={'Name':['Rachel','Ross','joey','chandler','monica','phoebe','tom','jerry','noddy','doremon','nobita','bheem','raju','moon','guru'],
          'Salary':[27173,22354,27930,28137,28053,21806,28366,27246,20452,24030,27008,24696,24297,23423,45452]}

df=pd.DataFrame(ser_dict)

df

df.columns

df=pd.read_csv('Data/Bank Churn.csv')

df.head()

df.tail()

df.shape

df.info()

df.describe()

df.head()

df.iloc[4:10,[0,1,2,3,6,7]]

df.loc[:,['CreditScore', 'Geography', 'Gender', 'Age','Tenure', 'Balance', 'NumOfProducts']]

df.columns

df[['CreditScore', 'Geography', 'Gender', 'Age','Tenure', 'Balance', 'NumOfProducts']]

df[['CreditScore']]

df.CreditScore

df[df['Gender']=='Male']

df=pd.read_csv('/content/Data/example.csv',index_col=['Month'])

df.head()

df.shape

df.info()

df.columns

df[df[' "1958"'].isnull()].index

df[df[' "1959"'].isnull()].index

df[df[' "1960"'].isnull()].index

df.drop(['APR', 'AUG'],axis=0)

df.drop(' "1958"',axis=1,inplace=True)

df.drop(df[df[' "1959"'].isnull()].index,axis=0)

df[df[' "1960"'].isnull()]

df[' "1960"'].dropna()

import pandas as pd

df=pd.read_excel('Data/Car_Data.xlsx',sheet_name='cars_ds_final')
df=df.iloc[:,:10]

df.head()

## Null values in %

df.isnull().sum()/len(df)*100

## Treating Null Values

df['Displacement'].mean(),df['Displacement'].median()

df['Cylinders'].mode()

df['Displacement'].fillna(df['Displacement'].mean(),inplace=True)
df['Make'].fillna(df['Make'].mode().values[0],inplace=True)
df['Cylinders'].fillna(df['Cylinders'].mode().values[0],inplace=True)
df['Valves_Per_Cylinder'].fillna(df['Valves_Per_Cylinder'].mode().values[0],inplace=True)
df['Drivetrain'].fillna(df['Drivetrain'].mode().values[0],inplace=True)
df['Cylinder_Configuration'].fillna(df['Cylinder_Configuration'].mode().values[0],inplace=True)
df['Engine_Location'].fillna(df['Engine_Location'].mode().values[0],inplace=True)

df.isnull().sum()/len(df)*100

df.head()

df.drop('isker',axis=1,inplace=True)

df.head()

df.rename(columns={'Valves_Per_Cylinder':'values_per_cylinder'})

df=pd.read_csv('/content/example.csv')
df.head()

df.columns

df.rename(columns={' "1958"':'1958',' "1959"':'1959',' "1960"':'1960'},inplace=True)

df.head()

df.columns

df.to_excel('test.xlsx',index=False)
df

df.to_csv('test1.csv',index=False)
df

df1=pd.read_csv('test1.csv')

df1.drop('Unnamed: 0',axis=1,inplace=True)

df1.head()

df=pd.read_csv('/content/Bank Churn.csv')

df.head()

{1:'Leave',0:'stay'}

df.loc[df['Exited']==1,'Exited']='Leave'

df.loc[df['Exited']==0,'Exited']='stay'

df.head()

df.loc[df['EstimatedSalary']>100000,'status']='Rich'
df.loc[df['EstimatedSalary']<100000,'status']='Poor'

import pandas as pd
df=pd.read_csv('/content/Bank Churn.csv')

df.head()

df['Geography'].unique()

df.shape

df.loc[df['Geography']=='fra','Geography']='France'
df.loc[df['Geography']=='france','Geography']='France'

df.loc[df['Geography']=='France']

df.sort_values('CreditScore',ascending=False)

df.Gender.unique()

df.loc[df['Gender']=='Female','Gender']=1
df.loc[df['Gender']=='Male','Gender']=0

df.head()

df['Gender'].replace(['Female','Male'],[1,0],inplace=True)


