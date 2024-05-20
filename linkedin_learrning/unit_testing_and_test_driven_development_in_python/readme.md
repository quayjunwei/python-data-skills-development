# unit_test_practice


## Example
```python
import pytest

# Production Code
def str_len(theStr):
    return len(theStr)

# A Unit Test
def test_string_length():
    testStr = "1" # set up
    result = str_len(testStr) # action
    assert result == 1 # assert
```
## Uncle Bob's 3 laws of TDD

- You may not write any production code until you have written a failing unit test.  
- You may not write more of a unit test than is sufficient to fail, and not compiling is failing.  
- You may not write more production code than is sufficient to pass the currently failing unit test.  