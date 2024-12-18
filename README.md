import random

def check(comp, user):
    if comp == user:
        return 0
    
    if (comp == 1 and user == 2):
        return -1
    
    if (comp ==2 and user ==3):
        return -1
    
    if (comp ==3 and user ==1):
        return -1
    
    return 1 


comp = random.randint(1,3)
user = int(input("1 for Scissors , 2 for Paper , 3 for Rock:\n "))


score = check(comp,user)
print("you: ",  user)
print("computer: ", comp)

if(score == 0):
    print("its a Draw")
elif score == 1:
    print("you won")

else:
    print("you lose")    
   

