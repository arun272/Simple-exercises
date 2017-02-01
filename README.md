# practice
f=open('ages.txt','r').readlines()
name = input("Name:")
name_found=False
for line in f:
    words=line.split(",")
    if words[0]==name:
        name_found=True
        print (words[1])
        break

if name_found is False:
    print("name not found")
