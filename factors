import sys

def factors(n):
    # Initialize list of factors
    factors = []

    # Divide n by 2 until it is odd
    while n % 2 == 0:
        factors.append(2)
        n = n // 2

    # Divide n by odd numbers until it is 1
    i = 3
    while n != 1:
        while n % i == 0:
            factors.append(i)
            n = n // i
        i += 2

    # Return the first two elements of the list
    return factors[0], factors[1]

# Read file name from command line
filename = sys.argv[1]

# Open file
with open(filename, 'r') as f:
    # Read numbers from file and factorize them
    for line in f:
        n = int(line.strip())
        p, q = factors(n)
        print(f'{n}={p}*{q}')

