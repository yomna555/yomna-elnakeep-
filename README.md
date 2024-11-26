# yomna-elnakeep-
https://drive.google.com/drive/folders/1wCpMm4qqhL-5xDa44NdcGRwtuPYtuOUx?usp=drive_link

first task
steps=input("enter your steps:")

steps_string=steps.split()

steps_string=list(map(int,steps_string))
highest_STEP=max(steps_string)
lowest_STEP=min(steps_string)
avg_STEPS=sum(steps_string)/len(steps_string)
steps_sorted_desc = sorted(steps_string, reverse=True)

print(f"Highest step count: {highest_STEP}")
print(f"Lowest step count: {lowest_STEP}")
print(f"Average daily step count: {avg_STEPS:.2f}")
print(f"Steps in descending order: {steps_sorted_desc}")
=========================================================================================================================================================================================
second task

records = [
    "Book A - 7",
    "Book B - 3",
    "Book A - 5",
    "Book C - 10",
    "Book D - 2",
    "Book B - 4",
]


books = {}


for record in records:
    title, days = record.split(" - ")
    days = int(days) 
    if title in books:  
        books[title] += days 
    else:  
        books[title] = days 


most_borrowed = max(books, key=books.get)  
least_borrowed = min(books, key=books.get) 
average_days = sum(books.values()) / len(books)  
unique_titles = set(books.keys())  
sorted_books = sorted(books.items(), key=lambda x: x[1], reverse=True)  


print(f"Most borrowed book: {most_borrowed} - {books[most_borrowed]} days")
print(f"Least borrowed book: {least_borrowed} - {books[least_borrowed]} days")
print(f"Average borrowing time: {average_days:.2f} days")
print(f"Unique book titles: {unique_titles}")
print("Books sorted by borrowed days:")
for title, days in sorted_books:
    print(f"{title}: {days} days")
====================================================================================================================
third 
import random
word=["yomna","hana","mariam","mohammed"]

Or_word=random.choice(word)

S_word=""
for char in random.sample(Or_word,len(Or_word)):
    S_word +=char
    
tries=5
while tries>0:
    guess=input("Enter your guess:")
    if guess==Or_word:
        print("congratulation!")
        break
    else:
        tries -=1
        print(f"try again you have {tries} try")
        
if tries==0:
    print(f"GAME OVER! the correct word is {Or_word}")

==================================================================================================================================================
