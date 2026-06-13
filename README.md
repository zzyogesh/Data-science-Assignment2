# Data-science-Assignment2
#  1.  Create a tuple: 
my_tuple = (10, 20, 30, 40, 50)
print(my_tuple[0])  # first element
print(my_tuple[-1])  # last element
print(len(my_tuple))  ## len of tuple
print(my_tuple[1:4])  # elements from index 1 to 3


# Q 2.   Create a tuple: 
fruits = ("apple", "banana", "mango", "orange")
print(fruits[1])  # second fruit
print(fruits[-2:])  # last two fruits
print(len(fruits))   # total number of fruits


# Q 3.  Create a set: 
numbers = {10, 20, 30, 40, 50}
print(numbers)  # # Complete set
print(len(numbers))  # # Length of the set
print(30 in numbers)   # # Check whether 30 is present in the set

# Q4.  Create two sets: 
set1 = {1, 2, 3, 4} 
set2 = {3, 4, 5, 6} 
print(set1|set2)  ##Union
print(set1&set2)  ##Intersection
  
#  Q 5. Create a dictionary: 
student = {"name":"Kriti", "age":20, "course":"Python"} 
print(student)  # Complete dictionary
print(student["name"])  # Student name
print(student["age"])  # Student age
print(student["course"])  # Student course

#  Create a list: 
numbers = [12, 45, 7, 23, 56, 89, 34] 
print(max(numbers))  # Largest element
print(sorted(numbers, reverse=True)[1])  # Second largest element
print(min(numbers))  # Smallest element
  
#  Q 6. Create a list: 
arr = [10, 20, 30, 40, 50, 60] 
# Write a function that takes the list as input
# and returns the list in reverse order without using the reverse() method
def reverse_list(lst):
    return lst[::-1]

print(reverse_list(arr))

#  Q 7. Create a tuple: 
data = (5, 10, 15, 20, 25, 30, 35) 

count = sum(1 for x in data if x % 5 == 0) 
total = sum(data)
average = total / len(data)
print(count)
print(total)
print(average)

#  Q 8. Create a dictionary: 
students = { 
    "Aman": 78, 
    "Riya": 92, 
    "Kriti": 88, 
    "Rahul": 95 
} 
# Write a program to: 


highest_student = max(students, key=students.get)
lowest_student = min(students, key=students.get)
high_scorers = {name: score for name, score in students.items() if score > 85}

print("Highest marks:", highest_student, students[highest_student])
print("Lowest marks:", lowest_student, students[lowest_student])
print("Students scoring more than 85:", high_scorers)


#  Q 9. Write a function:
# count_frequency(arr) that takes a list as input and prints the frequency of each element.

def count_frequency(arr):
    freq = {}
    for item in arr:
        freq[item] = freq.get(item, 0) + 1
    for item, count in freq.items():
        times = "time" if count == 1 else "times"
        print(f"{item} -> {count} {times}")

arr = [1, 2, 2, 3, 1, 4, 2]
count_frequency(arr)



#  10. Write a function:
# find_duplicates(arr) that takes a list as input and prints all duplicate elements present in the list.

def find_duplicates(arr):
    seen = set()
    duplicates = set()
    for item in arr:
        if item in seen:
            duplicates.add(item)
        else:
            seen.add(item)
    for item in sorted(duplicates):
        print(item)

print("Duplicate elements are:")
find_duplicates(arr)

