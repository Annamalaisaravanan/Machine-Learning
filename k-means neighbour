from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split 
import numpy as np
import pandas as pd
x,y=load_iris(return_X_y=True)
k=y.reshape(-1,1)
k.shape
print(x,my_data)
my_data=np.concatenate([x,k],1)
my_data
que=[float(i) for i in input().split(',')]
kd=int(input())
def distance(trainingset,test_insta):
    dis=0
    for j in range(0,x.shape[1]):
           dis+=pow((trainingset[j]-test_insta[j]),2)
    df=np.sqrt(dis)
    return df
def knn(x,que,k):
   tab=[]
   neighbour={}
   for i in range(0,my_data.shape[0]-1):
         dis=distance(x[i],que)
         tab.append((dis,x[i]))
   tab.sort(key=lambda x:x[0])
   for i in range(0,k):
     response=tab[i][-1][-1]
     if response in neighbour:
        neighbour[response]+=1
     else:
        neighbour[response]=1
   print(neighbour)
knn(my_data,que,kd)
