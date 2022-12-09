# python-project
#finding leap year and non leap year between given period of time
def leap(n):
    f=False
    if (n%100!=0 and n%4==0) or n%400==0:
        f=True
    return f
#to send the function's result back to the caller
*l,a=map(int,input().split('/'))
#to get multiple input values from user in one line
#split a string into a list
*l1,b=map(int,input().split('/'))
leapYears=[]
nonLeapYears=[]
for i in range(a,b+1):
    if leap(i):
        leapYears.append(i)
#at end of a list to add some items
    else:
        nonLeapYears.append(i)
print(leapYears)
print(nonLeapYears)
