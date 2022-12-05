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
