# chinchirorin
diceのレポジトリを繰り返しでまとめた。
from vpython import*

import random

a=random.randint(1,6)

b=random.randint(1,6)

c=random.randint(1,6 )

box(pos=vector(0,0,0),length=10,width=1,height=10,color=color.white)

box(pos=vector(0+2*11,0,0),length=10,width=1,height=10,color=color.white)

box(pos=vector(0+11,0,0),length=10,width=1,height=10,color=color.white)


di=[a,b,c]

for i in range (3):

    print(di)
    
    
    if di[i]==1:

        cylinder(pos=vector(0+11*i,0,0),axis=vector(0,0,1),radius=1,color=color.red)
        
    elif di[i]==2:

        cylinder(pos=vector(2.5+11*i,2.5,0),axis=vector(0,0,1),color=color.black) 

        cylinder(pos=vector(-2.5+11*i,-2.5,0),axis=vector(0,0,1),color=color.black)
    
    elif  di[i]==3:
    
        cylinder(pos=vector(0+11*i,0,0),axis=vector(0,0,1),radius=1,color=color.black)
        
       
        cylinder(pos=vector(2.5+11*i,2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(-2.5+11*i,-2.5,0),axis=vector(0,0,1),radius=1,color=color.black)  
        
    elif  di[i]==4:
   
        cylinder(pos=vector(2.5+11*i,-2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        
        cylinder(pos=vector(2.5+11*i,2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(-2.5+11*i,-2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(-2.5+11*i,2.5,0),axis=vector(0,0,1),radius=1,color=color.black)  
        

    elif  di[i]==5:


        cylinder(pos=vector(0+11*i,0,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(2.5+11*i,-2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(2.5+11*i,2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(-2.5+11*i,-2.5,0),axis=vector(0,0,1),radius=1,color=color.black)

        cylinder(pos=vector(-2.5+11*i,2.5,0),axis=vector(0,0,1),radius=1,color=color.black)    
        
    else:

        cylinder(pos=vector(2.5+11*i,0,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(2.5+11*i,-2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        
        cylinder(pos=vector(2.5+11*i,2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(-2.5+11*i,0,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(-2.5+11*i,-2.5,0),axis=vector(0,0,1),radius=1,color=color.black)
        
        cylinder(pos=vector(-2.5+11*i,2.5,0),axis=vector(0,0,1),radius=1,color=color.black)    
