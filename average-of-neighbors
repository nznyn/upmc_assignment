import numpy as np

#user prompts for size of the array
print("please enter dimensions as integer values >= 3")
x = int(input("enter x: "))
y = int(input("enter y: "))
z = int(input("enter z: "))

#user prompts for point in the array 
#preferably >= 1 and less than values for x, y, z
print()
print("please enter point in structure")
i = int(input("enter i: "))
j = int(input("enter j: "))
k = int(input("enter k: "))
print()

shape = (x, y, z)

#x is an array in the shape of user's choice
#of random integers between 0 and 5
x = np.random.randint(0, 6, shape)

print("array looks like this: \n")
print(x, "\n")

d = np.r_[i, j, k]

#function f slices 3 x 3 x 3 around central point "d" and
#prints the average of that slice
def f(x, d):
  idx = tuple(slice(d0 - 1, d0 + 2) for d0 in d)
  print("slice considered: \n")
  print(x[idx], "\n")
  print("average of 27 nearest neighbors of point d: \n", x[idx].mean())

#call to function f(x, d)
# sends function 3D array "x" and specified point "d" in array
f(x, d)
