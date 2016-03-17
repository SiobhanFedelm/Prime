# Prime

Anything below two is not prime number so we have to start by excluding them. 

Two is dealt with on its own line because in order for the metric by which we test other numbers for prime/not prime status to work we have to exclude division by two.

The return True is outside of the for loop because otherwise it will only test x against the first number in the range before providing an answer.

```

def is_prime(x):
    if x < 2:
        return False
    elif x == 2:
        return True
    elif x > 2:
        for n in range(2, x-1):
            if x % n == 0:
                return False
        else:
            return True
            
  ```
