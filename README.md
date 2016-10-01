# Algorithm
#Given integer A and B, calculate how many numbers falling in range [A, B] are perfect squares of another int. 
#Example  A = 4, B = 17, then return 3 because 2^2=4, 3^2=9, 4^2=16.

def PerfectSquares(a, b):
    count = 0 # initialize result
    # Traverse through all numbers
    for i in range (a,b+1):
        j = 1;
        while j*j <= i:
            if j*j == i:
                 count = count+1
            j = j+1
        i = i+1
    return count
Result=PerfectSquares(4,17)
