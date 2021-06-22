# Pthon
## Why Python
### Python installation and Pycharm set up

- Test installation and Pycharm

# To initialise a repo using pycharm

- ```git init```
- To check what's added to be sent to git hub
- ```git status``` to ensure only required files are added to be sent
- To add ```git add .``` or ```git add name_of_the_file```
- To save changes ```git commit -m "logical message" ```
- To push changes to git hub ```git push -u origin main```
- If you have not set remote branch to main
- You need to run ```git branch -M main``` after running the commit command
- Adding remote to connect localhost with github repo
- ```git remote add origin git@github.com:example/eng89_python_basics.git``` Setting the branch to -M main and adding the remote is only to be done first time

Diagram by Khanmaster
![Diagram by Khanmaster](https://trello-attachments.s3.amazonaws.com/603d260f5690ef1cd5b54430/60d05369263b542bdb3c3361/35665861b9b1a7ea274e0d5c8fb9d53d/Screenshot_(26).png)

# Activity/task

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
