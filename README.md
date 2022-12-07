# artificial-intelligence-and-machine-learning<br>
**program to calculate square root of a number**<br>
# Python Program to calculate the square root<br>
# Note: change this value for a different result<br>
num = 64<br>
# To take the input from the user<br>
#num = float(input('Enter a number: '))<br>
num_sqrt = num ** 0.5<br>
print('The square root of %0.3f is %0.3f'%(num ,num_sqrt))<br>
**output**
The square root of 64.000 is 8.000<br>

**solve quadratic equations**<br>
# import complex math module  <br>
import cmath  <br>
a = float(input('Enter a: '))  <br>
b = float(input('Enter b: '))  <br>
c = float(input('Enter c: '))   <br>
# calculate the discriminant  <br>
d = (b**2) - (4*a*c)    <br>
# find two solutions <br> 
sol1 = (-b-cmath.sqrt(d))/(2*a) <br> 
sol2 = (-b+cmath.sqrt(d))/(2*a)  <br>
print('The solution are {0} and {1}'.format(sol1,sol2))  <br> 
**output**<br>
Enter a: 10<br>
Enter b: 6<br>
Enter c: 4<br>
The solution are (-0.3-0.5567764362830021j) and (-0.3+0.5567764362830021j)<br>
**program to swap two varibles**<br>
# Python program to swap two variables<br>
x = 5<br>
y = 10<br>
# To take inputs from the user<br>
#x = input('Enter value of x: ')<br>
#y = input('Enter value of y: ')<br>
# create a temporary variable and swap the values<br>
temp = x<br>
x = y<br>
y = temp<br>
print('The value of x after swapping: {}'.format(x))<br>
print('The value of y after swapping: {}'.format(y))<br>
**output**<br>
The value of x after swapping: 10<br>
The value of y after swapping: 5<br>
**check armstrong number**<br>
# take input from the user<br>
num = int(input("Enter a number: "))<br>
# initialize sum<br>
sum = 0<br>
# find the sum of the cube of each digit<br>
temp = num<br>
while temp > 0:<br>
   digit = temp % 10<br>
   sum += digit ** 3<br>
   temp //= 10<br
# display the result<br>
if num == sum:<br>
   print(num,"is an Armstrong number")<br>
else:<br>
   print(num,"is not an Armstrong number")<br>
   **output**<br>
   Enter a number: 560<br>
560 is not an Armstrong number<br>
Enter a number: 407<br>
407 is an Armstrong number<br>
**Python program to find H.C.F of two numbers**<br>
# Python program to find H.C.F of two numbers<br>
# define a function<br>
def compute_hcf(x, y):<br>
# choose the smaller number<br>
    if x > y:<br>
        smaller = y<br>
    else:<br>
        smaller = x<br>
    for i in range(1, smaller+1):<br>
        if((x % i == 0) and (y % i == 0)):<br>
            hcf = i <br>
    return hcf<br>
num1 = 54 <br>
num2 = 24<br>
print("The H.C.F. is", compute_hcf(num1, num2))<br>
**output**<br>
The H.C.F. is 6<br>
**Python Program to find the L.C.M. of two input number**<br>
# Python Program to find the L.C.M. of two input number<br>
def compute_lcm(x, y):<br>
   # choose the greater number<br>
   if x > y:<br>
       greater = x<br>
   else:<br>
       greater = y<br>
<br>
   while(True):<br><br>
       if((greater % x == 0) and (greater % y == 0)):<br>
           lcm = greater<br>
           break<br>
       greater += 1<br>
   return lcm<br>
num1 = 54<br>
num2 = 24<br>
print("The L.C.M. is", compute_lcm(num1, num2))<br>
**output**<br>
The L.C.M. is 216<br>
**Program to add two matrices using nested loop**<br>
# Program to add two matrices using nested loop<br>
X = [[12,7,3],<br>
    [4 ,5,6],<br>
    [7 ,8,9]]<br>
Y = [[5,8,1],<br>
    [6,7,3],<br>
    [4,5,9]]<br>
result = [[0,0,0],<br>
         [0,0,0],<br>
         [0,0,0]]<br>
# iterate through rows<br>
for i in range(len(X)):<br>
   # iterate through columns<br>
   for j in range(len(X[0])):<br>
       result[i][j] = X[i][j] + Y[i][j]<br>
for r in result:<br>
   print(r)<br>
   **output**<br>
   [17, 15, 4]<br>
[10, 12, 9]<br>
[11, 13, 18]<br>
**program to sort dictionaries**<br>
dt = {5:4, 1:6, 6:3}<br>
sorted_dt = {key: value for key, value in sorted(dt.items(), key=lambda item: item[1])}<br>
print(sorted_dt)<br>
**output**<br>
{6: 3, 5: 4, 1: 6}<br>
or<br>
dt = {5:4, 1:6, 6:3}<br>

sorted_dt_value = sorted(dt.values())<br>
print(sorted_dt_value)<br>
**output**<br>
[3, 4, 6]<br>
**program to convert string to date and time**<br>
from datetime import datetime<br>
my_date_string = "Mar 11 2011 11:31AM"<br>
datetime_object = datetime.strptime(my_date_string, '%b %d %Y %I:%M%p')<br><br>
print(type(datetime_object))<br>
print(datetime_object)<br>
**output**<br>
<class 'datetime.datetime'><br>
2011-03-11 11:31:00<br>
**python program to reverse a numer**<br>
 
n=int(input("Enter number: "))<br>
rev=0<br>
while(n>0):<br>
    dig=n%10<br>
    rev=rev*10+dig<br>
    n=n//10<br>
print("Reverse of the number:",rev)<br>

