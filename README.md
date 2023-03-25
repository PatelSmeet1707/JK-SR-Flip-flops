2. JK Flip-Flop ===================================================================================================================================

i=0
while i<8:
    
    J = int(input('Enter state <0/1> :'))
    K = int(input('Enter state <0/1> :'))
    Qp = int(input('Enter state <0/1> :'))
    
    if J==0 and K==0 and Qp==0:
        ans=0
        print(ans,',Hold state')
    elif J==0 and K==0 and Qp==1:
        ans=1
        print(ans,',Hold state')
    elif (J==0 and K==1 and Qp==0) or (J==0 and K==1 and Qp==1):
        ans=0
        print(ans,',Reset state')
    elif (J==1 and K==0 and Qp==0) or (J==1 and K==0 and Qp==1):
        ans=1
        print(ans,',Set state')
    elif J==1 and K==1 and Qp==0:
        ans=1
        print(ans,',Toggle state')
    elif J==1 and K==1 and Qp==0:
        ans=0
        print(ans,',Toggle state')
    else:
        print("Enter correct values !")


3. SR Flip-Flop ===================================================================================================================================

i=0
while i<8:
    
    S = int(input('Enter state SET <0/1> :'))
    R = int(input('Enter state RESET <0/1> :'))
    Qp = int(input('Enter state <0/1> :'))
    
    if S==0 and R==0 and Qp==0:
        ans=0
        print(ans,',Hold state')
    elif S==0 and R==0 and Qp==1:
        ans=1
        print(ans,',Hold state')
    elif (S==0 and R==1 and Qp==0) or (S==0 and R==1 and Qp==1):
        ans=0
        print(ans,',Reset state')
    elif (S==1 and R==0 and Qp==0) or (S==1 and R==0 and Qp==1):
        ans=1
        print(ans,',Set state')
    elif S==1 and R==1 and Qp==0 or S==1 and R==1 and Qp==1:
        ans=1
        print(ans,',Indeterminate state')
    else:
        print("Enter correct values !")
