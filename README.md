import os
os.chdir("c:/BinaryFilesDemo")
fp=open("c:/BinaryFilesDemo/seperatechar.txt",'r')
#mylist=[1,22,"a","#","@","A"]
#fp.write(str(mylist))
aa=fp.read()
print("seperatechar.txt file data is :",aa)
myList1=list(aa)
lowerList=[]
upperList=[]
numList=[]
spclList=[]
for itr in myList1:
    #print(itr)
    if itr.isupper():
        upperList.append(itr)
        #print(upperList)
        #print(itr)
    elif itr.isnumeric():
        numList.append(itr)
        #print(numList)
        #print(itr)
    elif itr.islower():
        lowerList.append(itr)
        #print(lowerList)

        #print(itr)
    else:
        spclList.append(itr)
        #print(spclList)
print("upper case characters in file :",upperList)
print("Numbers in file :",numList)
print("lower case characters in file :",lowerList)
print("special characters in file :",spclList)

