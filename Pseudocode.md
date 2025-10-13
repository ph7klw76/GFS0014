# Pseudocode 

Pseudocode  is a step-by-step plan written in simple language that looks a bit like code but ignores exact syntax. 
For Python, keep indentation, use clear names, and write one action per line so translating to Python is easy.

'''text
# Problem: say what you’re solving.
# Inputs: what comes in?
# Output: what should come out?

DEFINE function_name(inputs)
    STEP 1
    STEP 2 (conditions / loops if needed)
    RETURN result
END
'''

## Example 1- sum of a list

```text
# Problem: Add up all numbers in a list
# Inputs: nums (list of numbers)
# Output: total (number)

DEFINE sum_list(nums)
    SET total TO 0
    FOR each n in nums
        SET total TO total + n
    ENDFOR
    RETURN total
END
```

Python
```python
def sum_list(nums):
    total = 0
    for n in nums:
        total += n
    return total
```

## Example 2 — Find the largest number

```text
# Problem: Return the maximum value in a list (assume list not empty)
# Inputs: nums (list)
# Output: max_value (number)

DEFINE find_max(nums)
    SET best TO first element of nums
    FOR each n in nums starting from second
        IF n > best
            SET best TO n
        ENDIF
    ENDFOR
    RETURN best
END
```

Python
```python
def find_max(nums):
    best = nums[0]
    for n in nums[1:]:
        if n > best:
            best = n
    return best
```

## Example 3 — Check if a number is even

```text
# Problem: Is x an even number?
# Inputs: x (integer)
# Output: True/False

DEFINE is_even(x)
    IF x modulo 2 equals 0
        RETURN True
    ELSE
        RETURN False
    ENDIF
END
```

python
```python
def is_even(x):
    if x % 2 == 0:
        return True
    else:
        return False
```

## Example 4 — Count vowels in a word

```text
# Problem: Count how many vowels are in a word
# Inputs: word (string)
# Output: count (integer)

DEFINE count_vowels(word)
    SET vowels TO set of {'a','e','i','o','u'}
    SET count TO 0
    FOR each character c in lowercase(word)
        IF c in vowels
            INCREMENT count
        ENDIF
    ENDFOR
    RETURN count
END
```

python
```python
def count_vowels(word):
    vowels = {'a','e','i','o','u'}
    count = 0
    for c in word.lower():
        if c in vowels:
            count += 1
    return count
```
