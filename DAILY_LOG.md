# Daily Learning Log

## Day 1 - 02.04.2026
## Day 2- 03.04.2026

#counting in a loop
i = 0
print("before",i)
for term in [11,21,31,41,51,61,71,81,91]:
    i = i+1
    print(term,i)
print("after",i)


#summing in a Loop
total = 0
print("before",total)
for item in [12,21,31,41,32,23,45]:
    total = total + item
    print(item,total)
print("after",total)

#taking the average in a Loop
sum = 0
counter = 0
for x in [5,15,22,32,13,73]:
    sum = sum + x
    counter = counter + 1
    print(x,counter,sum,sum/counter)

#filtering in a Loop
i = -1
for new in [5,3,65,23,42,30]:
    if new > i:
        i = new
        print(i)

#search using a Loop
found = False
#looking for 23
for item in [42,89,23,98,14,24,45]:
    if item == 23:
        print(item,True)
    else:
        print(item,found)  

#finding the smallest value in a Loop
bool=False
i = 45
print("here comes the value to compare",i)
for new in [4,23,45,12,76,88,-4]:
    if new < i:
        bool=True
        print(new,True)
    else:
        print(new,False)

#finding the smallest value in a Loop using None
smallest = None
for i in [12,21,43,-5,23,-54,0]:
    if smallest == None:
        print(smallest)
        smallest = i
    elif i<smallest:
        smallest = i
        print(i)
