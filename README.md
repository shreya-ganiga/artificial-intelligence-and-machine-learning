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
**output**<br>
Enter number: 43761<br>
Reverse of the number: 16734<br>
**python program to  compute power of a number**<br>
base = 3<br>
exponent = 4<br>
result = 1<br>
for exponent in range(exponent, 0, -1):<br>
    result *= base<br>
print("Answer = " + str(result))<br>
**output**<br>
Answer = 81<br>
**python program to create count down timer**<br>
import time<br>
def countdown(time_sec):<br>
    while time_sec:<br>
        mins, secs = divmod(time_sec, 60)<br>
        timeformat = '{:02d}:{:02d}'.format(mins, secs)<br>
        print(timeformat, end='\r')<br>
        time.sleep(1)<br>
        time_sec -= 1<br>
    print("stop")<br>
countdown(60)<br>
**output**<br>
stop1<br>
**python program to convert byte to a string**<br>
print(b'Easy \xE2\x9C\x85'.decode("utf-8"))<br>
**output**<br>
Easy ✅<br>
**lablist program**<br>
**breadth first search**<br>
graph = { <br>
'1' : ['2','10'], <br>
'2' : ['3','8'], <br>
'3' : ['4'], <br>
'4' : ['5','6','7'], <br>
'5' : [], <br>
'6' : [], <br>
'7' : [], <br>
 '8' : ['9'], <br>
'9' : [], <br>
'10' : [] <br>
 } <br>
visited = []  <br>
queue = []  <br>
def bfs(visited, graph, node): <br>
 visited.append(node) <br>
 queue.append(node) <br>
 while queue:  <br>
  m = queue.pop(0)  <br>
  print (m, end = " ")  <br>
  for neighbour in graph[m]: <br>
   if neighbour not in visited:  <br>
    visited.append(neighbour) <br>
    queue.append(neighbour) <br>
print("Following is the Breadth-First Search")<br>
<br>
bfs(visited, graph, '1')  <br>
**output**<br>
Following is the Breadth-First Search<br>
1 2 10 3 8 4 9 5 6 7 <br>
**depth first search**<br>
 graph = { <br>
 '5' : ['3','7'], <br>
 '3' : ['2', '4'], <br>
 '7' : ['6'], <br>
 '6': [], <br>
 '2' : ['1'], <br>
 '1':[], <br>
 '4' : ['8'], <br>
 '8' : [] <br>
} <br>
visited = set() # Set to keep track of visited nodes of graph.    <br>
def dfs(visited, graph, node):   #function for dfs <br>
  if node not in visited: <br>
    print (node) <br>
    visited.add(node) <br>
    for neighbour in graph[node]: <br>
        dfs(visited, graph, neighbour)<br> 
# Driver Code <br>
print("Following is the Depth-First Search") <br>
dfs(visited, graph, '5')<br>
**output**<br>

Following is the Depth-First Search<br>
5<br>
3<br>
2<br>
1<br>
4<br>
8<br>
7<br>
6<br>
**water jug problem**<br>

from collections import defaultdict <br>
jug1, jug2, aim = 4, 3, 2 <br>
visited = defaultdict(lambda: False) <br>
def waterJugSolver(amt1, amt2): <br>
 if (amt1 == aim and amt2 == 0) or (amt2 == aim and amt1 == 0): <br>
  print(amt1, amt2) <br>
  return True <br>
 if visited[(amt1, amt2)] == False: <br>
  print(amt1, amt2) <br>
  visited[(amt1, amt2)] = True <br>
  return (waterJugSolver(0, amt2) or <br>
    waterJugSolver(amt1, 0) or <br>
    waterJugSolver(jug1, amt2) or <br>
    waterJugSolver(amt1, jug2) or <br>
    waterJugSolver(amt1 + min(amt2, (jug1-amt1)), <br>
    amt2 - min(amt2, (jug1-amt1))) or <br>
    waterJugSolver(amt1 - min(amt1, (jug2-amt2))<br>, 
    amt2 + min(amt1, (jug2-amt2)))) <br>
 else: <br>
  return False <br>
print("Steps: ") <br>
waterJugSolver(0, 0)<br>
**output**<br>

Steps: <br>
0 0<br>
4 0<br>
4 3<br>
0 3<br>
3 0<br>
3 3<br>
4 2<br>
0 2<br>
True<br>
**tower of hanoi**<br>
def TowerOfHanoi(n , source, destination, auxiliary): <br>
    if n==1:<br> 
        print ("Move disk 1 from source",source,"to destination",destination)<br><br>
        return <br>
    TowerOfHanoi(n-1, source, auxiliary, destination) <br>
    print ("Move disk",n,"from source",source,"to destination",destination)<br> 
    TowerOfHanoi(n-1, auxiliary, destination, source) <br>
n = 3 <br>
TowerOfHanoi(n,'A','B','C') <br>
**output**<br>

Move disk 1 from source A to destination B<br>
Move disk 2 from source A to destination C<br>
Move disk 1 from source B to destination C<br>
Move disk 3 from source A to destination B<br>
Move disk 1 from source C to destination A<br>
Move disk 2 from source C to destination B<br>
Move disk 1 from source A to destination B<br>
**best first search**<br>

from queue import PriorityQueue <br>
import matplotlib.pyplot as plt <br>
import networkx as nx <br>
# for implementing BFS | returns path having lowest cost def best_first_search(source, target, n): <br>
def best_first_search(source, target, n):<br>
 visited = [0] * n <br>
 visited[source] = True <br>
 pq = PriorityQueue()<br> 
 pq.put((0, source)) <br>
 while pq.empty() == False: <br>
  u = pq.get()[1] <br>
  print(u, end=" ") # the path having lowest cost <br>
  if u == target: <br>
     break<br>
    
 for v, c in graph[u]:  <br>
   if visited[v] == False:  <br>
     pq.put((c, v)) <br> 
print()  <br>
# for adding edges to graph  <br>
def addedge(x, y, cost):  <br>
  graph[x].append((y, cost))  <br>
  graph[y].append((x, cost)) <br>

v = int(input("Enter the number of nodes: ")) <br>
graph = [[] for i in range(v)] # undirected Graph <br>
e = int(input("Enter the number of edges: "))  <br>
print("Enter the edges along with their weights:")  <br>
for i in range(e):  <br>
  x, y, z = list(map(int, input().split()))  <br>
  addedge(x, y, z)  <br>
    
source = int(input("Enter the Source Node: "))  <br>
target = int(input("Enter the Target/Destination Node: ")) <br>
print("\nPath: ", end = "")  <br>
best_first_search(source, target, v)  <br>
**output** <br>

Enter the number of nodes: 4 <br>
Enter the number of edges: 5 <br>
Enter the edges along with their weights: <br>
0 1 1 <br>
0 2 1 <br>
0 3 2 <br>
2 3 2 <br>
1 3 3 <br>
Enter the Source Node: 2 <br>
Enter the Target/Destination Node: 1 <br>

Path: 2  <br>




