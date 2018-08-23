# python-study
age_of_sunny = 22
count = 0
while count <3:
    guess_age = int(input("guess_age:"))
    if guess_age == age_of_sunny:
        print("yes,you got it.")
        break
    elif guess_age>age_of_sunny:
        print("think smaller ...")
    else:
        print("think bigger!")
    count +=1
    if  count == 3:
        continue_confirm = input("do you want to keep guessing..?")
        if continue_confirm !='n':
            count =0
else:
    print("you have tried too many times..")
