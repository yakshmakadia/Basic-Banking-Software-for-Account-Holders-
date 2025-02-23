id=input("Enter id=") 
pswd=int(input("Enter password=")) 
print("\n") 
data={"virat":1234,"hardik":1111,"rahul":0000,"rohit":1212} 
data2={"virat":9865,"hardik":6464,"rahul":1656,"rohit":4532} 
ans2='y' 
if(pswd==data[id]): 
print("Welcome ",id,"!") 
while(ans2=='y' or ans2=="Y"): 
ans=int(input("How may we help you\n1>Press 1 for balance 
check\n2>Press 2 for deposit\n3>Press 3 for Withdrawal\n4>Press 4 to 
exit\nEnter here=")) 
print("\n") 
if(ans==1): 
print("Current balance is=",data2[id]) 
ans2=input("Need more help=") 
print("\n") 
elif(ans==2): 
dep=int(input("Enter amount=")) 
key=int(input("Enter password again=")) 
print("\n") 
if(key==pswd): 
a=data2[id]+dep 
data2.update({id:a}) 
print("Transaction Success!") 
print("Current balance is=",data2[id]) 
ans2=input("Need more help=") 
print("\n") 
else: 
print("wrong password") 
ans2=input("Need more help=") 
elif(ans==3): 
wed=int(input("Enter amount=")) 
print("\n") 
key=int(input("Enter password again=")) 
if(key==pswd): 
a=data2[id]-wed 
data2.update({id:a}) 
print("Transaction Success!") 
print("Current balance is=",data2[id]) 
ans2=input("Need more help=") 
print("\n") 
else: 
print("wrong password") 
ans2=input("Need more help=") 
print("\n") 
elif(ans==4): 
print("Thank you!") 
break
