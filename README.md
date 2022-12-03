# codingMania
new repo
b=input("Hi. This Program will Help You distribute your Cake :)")
d= int(input("Enter Cake Diameter(cm): "))
h=int(input("How Tall your Cake is(cm): "))
w=int(input("How heavy the cake is(gms): "))
vol = 3.14*((d/2)**2)*h
den=w/vol
print("press 1: For unequal pieces")
print("press 2: For equal pieces")
ch=input()
n=int(input("Enter the number of pieces you want:"))
x=(vol/n)*den
if ch=="1":
    print("press 1:if you want Uniquely sized Pieces")
    print("press 2:if you want Randomly sized pieces ")
    s=input()
    if s=="1":
        if n<27 or n<=26:
            print("It is possible")
        else:
            print("not possible")
    elif(s=="2"):
        if n<=360:
            print("Its possible")
        else:
            print("not possible")
elif(ch=="2"):
    if 360%n==0:
        print("Possible, and every piece will be",  "%.2f" %x,  "gms ")
    else:
        print("not possible")
