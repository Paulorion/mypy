---
id: 12kys
name: Test doc
file_version: 1.1.0
app_version: 1.0.3
file_blobs:
  mypy/api.py: 589bfbbfa1a7c5517931cf04c8a89af72fa25146
  CONTRIBUTING.md: 703e7df148f01ea994e21cdf85e2d57c07a0ee38
---

```
Wtf
```

<br/>

<br/>

This is my favorite code uwu
<!-- NOTE-swimm-snippet: the lines below link your snippet to Swimm -->
### 📄 mypy/api.py
```python
🟩 76     def run_dmypy(args: list[str]) -> tuple[str, str, int]:
🟩 77         from mypy.dmypy.client import main
🟩 78     
🟩 79         # A bunch of effort has been put into threading stdout and stderr
🟩 80         # through the main API to avoid the threadsafety problems of
🟩 81         # modifying sys.stdout/sys.stderr, but that hasn't been done for
🟩 82         # the dmypy client, so we just do the non-threadsafe thing.
🟩 83         def f(stdout: TextIO, stderr: TextIO) -> None:
🟩 84             old_stdout = sys.stdout
🟩 85             old_stderr = sys.stderr
🟩 86             try:
🟩 87                 sys.stdout = stdout
🟩 88                 sys.stderr = stderr
🟩 89                 main(args)
🟩 90             finally:
🟩 91                 sys.stdout = old_stdout
🟩 92                 sys.stderr = old_stderr
🟩 93     
🟩 94         return _run(f)
```

<br/>

`📄 CONTRIBUTING.md`

From `📄 CONTRIBUTING.md` take this

<br/>

Don't do what I did
<!-- NOTE-swimm-snippet: the lines below link your snippet to Swimm -->
### 📄 CONTRIBUTING.md
```markdown
🟩 41     ### Running tests
🟩 42     
🟩 43     Running the full test suite can take a while, and usually isn't necessary when
🟩 44     preparing a PR. Once you file a PR, the full test suite will run on GitHub.
🟩 45     You'll then be able to see any test failures, and make any necessary changes to
🟩 46     your PR.
🟩 47     
🟩 48     However, if you wish to do so, you can run the full test suite
🟩 49     like this:
```

<br/>

D othis

<br/>


<!-- NOTE-swimm-snippet: the lines below link your snippet to Swimm -->
### 📄 CONTRIBUTING.md
```markdown
🟩 54     You can also use `tox` to run tests (`tox` handles setting up the test environment for you):
🟩 55     ```
🟩 56     tox -e py
🟩 57     
🟩 58     # Or some specific python version:
🟩 59     tox -e py39
🟩 60     
🟩 61     # Or some specific command:
🟩 62     tox -e lint
```

<br/>

<br/>

<br/>


<!-- NOTE-swimm-snippet: the lines below link your snippet to Swimm -->
### 📄 CONTRIBUTING.md
```markdown
🟩 65     Some useful commands for running specific tests include:
🟩 66     ```bash
🟩 67     # Use mypy to check mypy's own code
🟩 68     python3 runtests.py self
🟩 69     # or equivalently:
🟩 70     python3 -m mypy --config-file mypy_self_check.ini -p mypy
🟩 71     
🟩 72     # Run a single test from the test suite
🟩 73     pytest -n0 -k 'test_name'
🟩 74     
🟩 75     # Run all test cases in the "test-data/unit/check-dataclasses.test" file
🟩 76     pytest mypy/test/testcheck.py::TypeCheckSuite::check-dataclasses.test
🟩 77     
🟩 78     # Run the linter
🟩 79     flake8
🟩 80     
🟩 81     # Run formatters
🟩 82     black . && isort .
🟩 83     ```
```

<br/>

<br/>

<br/>

DSfadsjlkfsjakflsdjafkladsjfkl `📄 CONTRIBUTING.md`
<!-- NOTE-swimm-snippet: the lines below link your snippet to Swimm -->
### 📄 CONTRIBUTING.md
```markdown
🟩 92     In particular, look for:
🟩 93     - [good first issues](https://github.com/python/mypy/labels/good-first-issue)
🟩 94     - [good second issues](https://github.com/python/mypy/labels/good-second-issue)
🟩 95     - [documentation issues](https://github.com/python/mypy/labels/documentation)
🟩 96     
🟩 97     You do not need to ask for permission to work on any of these issues.
🟩 98     Just fix the issue yourself, [try to add a unit test](#running-tests) and
🟩 99     [open a pull request](#submitting-changes).
🟩 100    
🟩 101    To get help fixing a specific issue, it's often best to comment on the issue
🟩 102    itself. You're much more likely to get help if you provide details about what
🟩 103    you've tried and where you've looked (maintainers tend to help those who help
🟩 104    
🟩 105    
```

<br/>

This file was generated by Swimm. [Click here to view it in the app](https://app.swimm.io/repos/Z2l0aHViJTNBJTNBbXlweSUzQSUzQVBhdWxvcmlvbg==/docs/12kys).