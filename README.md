def isEmpty(Arr):
    if len(Arr)==0:
        return True
def PUSH(Arr, item):
    if item%5==0:
        Arr.append(item)
        top=len(Arr)-1
        
def SHOW(Arr):
    if isEmpty(Arr):
        print('No item found')
    else:
        for i in Arr[::-1]:
                print(i)
Arr=[]
top=None
while True:
    print('****** IMPLEMENTATION OF PUSH IN STACK USING LIST ******')
    print('1: PUSH')
    print('2: SHOW')
    print('0: Exit')
    ch=int(input('Enter your choice:'))
    if ch==1:
        val=int(input('Enter a number to push:'))
        PUSH(Arr, val)
    elif ch==2:
        SHOW(Arr)
    elif ch==0:
        print('Bye')
        break
