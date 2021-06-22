# Pthon
## Why Python
### Python installation and Pycharm set up

- Test installation and Pycharm

#Activity/task

- variables first_name, last_name, age, DOB
- prompt user to input above value
- print/display the type of each value received from the user
- then display the data back to user with greeting message

```python

# variables first_name, last_name, age, DOB
# prompt user to input above value
full_name = input("Please enter your full name: ")
first_name, *last_name = full_name.split()
age = int(input("{} please enter your age: ".format(first_name)))
DOB = input("{} please enter your date of birth: ".format(first_name))


# print/display the type of each value received from the user
# then display the data back to user with greeting message
print("First Name = {first}".format(first=first_name) +  " >> Is type: ")
print(type(first_name))
#First Name= Ron Is type:
#<class 'str'>

print("Last Name = {last}".format(last=" ".join(last_name)) +  " >> Is type: ")
print(type(last_name))
#Last Name = Urbon >> Is type:
#<class 'list'>

print("Age = {}".format(age) +  " >> Is type: ")
print(type(age))
#Age = 24 >> Is type:
#<class 'str'>

print("Date of Birth = {}".format(DOB) +  " >> Is type: ")
print(type(DOB))
#Date of Birth = 01.02.1997 >> Is type:
#<class 'str'>

greetings = "Hello World!"
print(greetings[6:])
print(greetings[-6:])
```