# CSCI 185 Spring 2021
# Homework 6

# Due: 11:59 PM 03/15/2020

# Step 1: Please use the correct Unix commands and VI/VIM to complete the following four tasks in your terminal:
# Q1: Create a new folder named csci185hw_6 and cd to this new folder. 
# Q2: Use VI/VIM text editor to create and edit the makefile file to:
+ Create target 1(you can name it whatever you want) to find the difference between 1.txt and 2.txt
+ Create target 2(you can name it whatever you want) to append several lines of strings to 1.txt
+ Create target 3(you can name it whatever you want) to append several lines of strings(which should be different from 1.txt ) to 2.txt
+ Create target **clean** to remove 1.txt and 2.txt
# Q3: **make** target 1
# Q4: **make** target **clean**

+ Note: you may have some error like
~~~
make: *** [target1] Error 1
~~~
+ It is because of the exit code 1 by diff, which means there is difference between 1.txt and 2.txt
+ But an exit code 0 (which means successuful, we will learn this in topic 8) is needed for make and makefile.
+ To fix it, you can add "|| exit 0" to the diff command(|| means or operation, we will learn this in topic 8)
~~~
diff 1.txt 2.txt || exit 0
~~~



# Step 2: Please screen shot your terminal with the above 4 tasks
# Step 3: Please save the 4 screenshots in a PDF file, name it as "CSCI185_Homework6_JohnDoe(0123456).pdf", where 0123456 is your BeeCard number, and sumbit it on [Blackboard](https://blackboard.sau.edu/webapps/login/)
