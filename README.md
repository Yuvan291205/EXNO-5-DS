# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 ```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
![image](https://github.com/user-attachments/assets/a566f423-141f-47f2-8750-3ab091a53465)
```
import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph!')
plt.show()
```
![image](https://github.com/user-attachments/assets/52f38ff1-645c-47d1-bb09-1c2ebeeec105)
```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/724f299d-556f-43b0-b0e9-cb2c250b3692)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```
![image](https://github.com/user-attachments/assets/a365aacd-d6e7-4378-abfe-d1a8f35cae28)
```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![image](https://github.com/user-attachments/assets/31420675-bd16-424e-9385-83c198de1560)
```
years=[2010,2011,2012,2013,2014,2015]
yeild_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yeild_apples)
```
![image](https://github.com/user-attachments/assets/27df4fd2-eb66-4ba9-97f9-14e661cb0887)
```
years=range(2000,2012)
apples= [0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)');
```
![image](https://github.com/user-attachments/assets/0f1142f4-0c3c-4194-a943-716466a73413)
```
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)')
plt.title("Crop Yeilds in Kanto")
plt.legend(['Apples','Oranges']);
```
![image](https://github.com/user-attachments/assets/a53ad8fe-345a-41a0-a714-c10848adb747)
```
years=[2010,2011,2012,2013,2014,2015]
yeild_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yeild_apples)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)');
```
![image](https://github.com/user-attachments/assets/41b96f91-4380-4c58-a6a7-3ca7f10d219e)
```
years=range(2000,2012)
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yeild of Oranges (tons per hectare)");
```
![image](https://github.com/user-attachments/assets/39635b14-8014-4e96-a428-e0f2a7e7cecd)
```
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)')
plt.title("Crop Yeilds in Kanto")
plt.legend(['Apples','Oranges']);
```
![image](https://github.com/user-attachments/assets/f71f7c8e-5007-4e08-9feb-9857978852c4)
```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="blue")
plt.show()
```
![image](https://github.com/user-attachments/assets/ae101946-7215-4f7a-8acd-d591b27a69db)
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
y array([11, 12, 13, 14, 15, 16, 17, 18, 19, 20])
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/00b3b9fe-aecd-423b-a4b4-1e435aa9735e)
```
y=x*x y
array([ 0, 1, 4, 9, 16, 25, 36, 49, 64, 81])
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
![image](https://github.com/user-attachments/assets/a7673912-4c7e-49cf-a294-d40151c12028)
```
np.pi
3.141592653589793
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![image](https://github.com/user-attachments/assets/df886fe7-b835-45e2-94d5-2c07dc1b52fb)
```
import matplotlib.pyplot as plt
import numpy as np x=[1,2,3,4,5] y1=[10,12,14,16,18] y2=[5,7,9,11,13] y3=[2,4,6,8,10]
plt.fill_between(x,y1,color="blue")
plt.fill_between(x,y2,color="green")
plt.plot(x,y1,color="red")
plt.plot(x,y2,color="black")
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/120d8e11-c12c-4e36-a3f5-3e4e0d6eafa7)
```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![image](https://github.com/user-attachments/assets/d52b1a57-47eb-4c2a-ba00-92a3ccc9e99f)
```
x=[2,8,10] y=[11,16,9] x2=[3,9,11] y2=[6,15,11]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/19dd28e4-9281-4168-96fc-2dee5a8a8d3b)
```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40] range=(0,100) bins=10 plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8) plt.xlabel('age') plt.ylabel('No.of people') plt.title('My histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/1baf6cd2-cb5d-4512-bce5-cb1eb9d33cc2)
```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/95a6e2ed-1c77-48ef-b0a4-2790fd9e98ba)
```
fig,ax=plt.subplots() ax.boxplot(data) ax.set_xlabel('Data') ax.set_ylabel('Values') ax.set_title('Box plot')
```
![image](https://github.com/user-attachments/assets/fee1ae08-dc97-46fa-ad90-ab0b619cc2e8)
```
labels='Python','C++','Ruby','Java' sizes=[215,130,245,210] colors=['gold','yellowgreen','lightcoral','lightskyblue'] explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors, autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/cecc99d7-47b3-499b-8d49-080670ef3caf)
```
activities=['eat','sleep','work','play'] slices=[3,7,8,6] colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors, startangle=90,shadow=True,explode=(0,0,0.1,0), radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/user-attachments/assets/48de06c1-bd94-4a6e-9100-49f744ed8f56)

# Result:
 To Perform Data Visualization using matplot python library for the given datas is successful.
