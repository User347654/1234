numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
primes = []
not_primes = []
for j in numbers:
    is_primes = True
    for i in range(2,j):
        if j % i == 0:
           print(j, 'is Not Prime')
           is_primes = False
           not_primes.append(j)
           break
    if is_primes == True:
        primes.append(j)
        print(j, 'is prime')
primes.remove(1)
print('primes:', primes)
print('not primes:', not_primes
