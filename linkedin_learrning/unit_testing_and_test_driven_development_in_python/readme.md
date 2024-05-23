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

## CLI flags

| Flag                  | Description                                                  |
|-----------------------|--------------------------------------------------------------|
| `-v`, `--verbose`     | Increase verbosity, giving more detailed test output.        |
| `-q`, `--quiet`       | Decrease verbosity, showing less output during test runs.    |
| `--lf`, `--last-failed` | Only rerun the tests that failed at the last run.           |
| `--ff`, `--failed-first` | Run all tests but run the last failures first.            |
| `-k EXPRESSION`       | Only run tests which match the given substring expression.   |
| `-m MARKEXPR`         | Only run tests matching given mark expressions.              |
| `--durations=N`       | Show N slowest setup/test durations (N can be an integer).   |
| `--maxfail=num`       | Stop after the first num failures.                           |
| `--cov`               | Measure code coverage for tests.                             |
| `--html=report.html`  | Generate a HTML report for the test session.                 |
| `-x`, `--exitfirst`   | Exit instantly on first error or failed test.                |
| `--collect-only`      | Only collect tests, do not execute them.                     |  

Write only one assertion per test  
- Makes CI easier when test fails  

Tests shouldnt rely on other tests  
- should be isolated  
- use teardown code/function  

