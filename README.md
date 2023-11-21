import cv2
import os
import string
img=cv2.inread(“plant.png")
msg=input("enter a secret message")
password=input("enter a password")
d={}
c={}
for i in range(255):  
    d[chr(i)]=i
    c[i]=chr(i)
n=0;
m=0;
z=0
pas=input("enter passcode for decryption")
if(password==pas):  
for i in range(len(msg)):    
    message=message+c[img[n,m,z]]    
    n=n+1    
    m=m+1   
     z=(z+1)%3 
 print("decrypted message=",message)
else:   
 print("you are not authenticated")
![image](https://github.com/nandual/nandual/assets/151628363/8fe81c44-3656-4f43-9284-5e050f824151)


![image](https://github.com/nandual/nandual/assets/151628363/90cd9445-a778-46a7-bff7-b916bea3fd35)

 
