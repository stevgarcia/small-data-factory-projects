## 📖 Project Overview

# Sort an array

<img width="1425" height="903" alt="image" src="https://github.com/user-attachments/assets/c24832aa-f8a9-438d-a023-320e2a1e062e" />


The set variable has the array
the set variable Iteration has the expression builder @range(0,add(length(variables('InputArray')),-1))
The until cycle controls the iteration until @empty(variables('Iteration'))

<img width="1026" height="717" alt="image" src="https://github.com/user-attachments/assets/0c9ecf69-fbbd-4f01-a3e7-b4b567d0a2a5" />

# Inside the iteration 

We set the variable currentIndex @string(variables('Iteration')[0])
We set the varible nextIndex @string(add(int(variables('Iteration')[0]),1))


<img width="1094" height="328" alt="image" src="https://github.com/user-attachments/assets/3596a524-6c5b-4186-9a1d-edf7c97df32b" />

# The if condition

evaluates if the number is bigger or not
@greater(variables('InputArray')[int(variables('CurrentIndex'))],variables('InputArray')[int(variables('NextIndex'))])

if is true

<img width="1015" height="205" alt="image" src="https://github.com/user-attachments/assets/dfd26832-0118-45ea-a021-c9f425b0ac49" />


it takes the left and right side of the array
it swapps the array and then creates the Json format
updated the input array and resets the iteration

if is not true 

makes a skip and updates the iteration

<img width="688" height="323" alt="image" src="https://github.com/user-attachments/assets/d7086871-38c3-4b95-868e-a18bcdae9206" />
