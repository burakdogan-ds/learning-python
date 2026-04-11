## Day 11- 11.04.2026
#Histogram - Taking in a Numerical and Algorithmic Way
counts = dict()
line = input("Enter a line of text")
words = line.split()
for word in words:
    counts[word] = counts.get(word,0)+1
print("Counts",counts)

## Day 10- 10.04.2026
 #Word controller
 reeder = open("C:\\Users\\avdrb\\Desktop\\romeo.txt")
 mylist = list()
 for i in reeder:
     kelimeler = i.split()
     for kelime in kelimeler:
         if kelime not in mylist:
             mylist.append(kelime)
 print(mylist)
 #Text Organizer
reeder = open("C:\\Users\\avdrb\\Desktop\\mbox-short.txt")
count = 0
# 'line' is a much clearer variable name here
for line in reeder:
        # Look for 'From ' with a space to avoid 'From:' lines
    if line.startswith("From "):  
        # Split the line into a list of words
        words = line.split()    
        # The email address is always the second word (index 1)
        email = words[1]      
        # Print the email address (as usually requested by this assignment)
        print(email)       
        # Increment the counter
        count = count + 1
# Close the file when you are done
reeder.close()
print("There were", count, "lines in the file with From as the first word")

## Day 9- 09.04.2026
#Manipulating a File
try:
    asker = input("Write down the filename")
    myfile = open(asker)
    count=0
    mus=0
    for linereader in myfile:
        if linereader.startswith("X-DSPAM-Confidence:"):
            zorzer = linereader[-8:].rstrip()
            zorzer = float(zorzer)
            count=count+1
            mus=mus+zorzer            
        else:
            continue
    print("Average spam confidence:", mus/count)
except: 
    print("Wrong filename")
    # Collections
new_list = list()
new_list.append("sth")
print(new_list)
new_list.append("another thing")
print(new_list)
"sth" in new_list
"another thing" not in new_list
new_list.sort()
print(new_list)
nums = [3,2,54,65,76,87,98]
print(len(nums))
print(max(nums))
print(sum(nums))
numlist = list()
while True :
    inp = input("Write down a number")
    if inp == "done": break
    value = float(inp)
    numlist.append(value)
avg = sum(numlist) / len(numlist)
print(avg)
summ = 0
count = 0
while True:
    girdi = input("write down a number")
    if girdi == "done": break
    count = count + 1
    value = float(girdi)
    summ = summ + value
print("average is: ", summ/count)
abc = "with three words"
splitted = abc.split()
print(splitted)
for vav in splitted:
    print(vav)
reader = open("C:\\Users\\avdrb\\Desktop\\mbox-short.txt")
for i in reader:
    i = i.rstrip()
    if not i.startswith("From "): continue
    words = i.split()
    print(words[0:2])

## Day 8- 08.04.2026
## Day 7- 07.04.2026
## Day 6- 06.04.2026
## Day 5- 05.04.2026

## Day 4- 04.04.2026
#Searching Through a File
fhand = open("C:\\Users\\avdrb\\Desktop\\metin.txt")
for line in fhand:
    if line.startswith("From"):
        print(line)

#Reading a file
fhand = open("C:\\Users\\avdrb\\Desktop\\metin.txt")
okuyucu = fhand.read()
okuyucu

#Line count in a file
fhand = open("C:\\Users\\avdrb\\Desktop\\metin.txt")
count = 0
for line in fhand:
    count = count + 1
print("Line count is",count)

#Reading a File
fhand = open("C:\\Users\\avdrb\\Desktop\\metin.txt")
fhand
for okuyucu in fhand:
    print(okuyucu)

#Counting letters in a string
vava = input("Write down a word contains a")
count = 0
for i in vava:
    if i=="a":
        count = count + 1 
print(count)

#finding largest in a loop
largest = None
smallest = None
while True:
    # 1. Get the input as text
    num_input = input("Enter a number: ")
    # 2. Check if they want to quit FIRST
    if num_input == "done":
        break      
    # 3. Try to convert to an integer inside the loop
    try:
        num = int(num_input)
    except:
        print("Invalid input")
        continue  # 'continue' skips the rest of the loop and asks for input again
    # 4. Safe comparison (None check is on the left!)
    if largest is None or num > largest:
        largest = num
print(largest)

## Day 3- 03.04.2026
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
## Day 2 - 02.04.2026
## Day 1 - 01.04.2026



        
