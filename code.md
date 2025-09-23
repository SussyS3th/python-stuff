# September 23, 2025 - first real coding proiblem i solved in python
# solves 1/(x+1/(x+1/(x+1)))/x

x = float(input("Enter value for x: "))
y = 1 / (x+1 /(x+1/ (x+1))) / x
print("y =", y)

# OR

x = float(input("Enter value for x: "))
print("y =",str( 1 / (x+1 /(x+1/ (x+1))) / x))
