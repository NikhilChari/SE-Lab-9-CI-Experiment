# SE Lab 9 — Introduction to Continuous Integration (CI)

**Student:** Nikhil Chari  
**Roll No.:** 24P0051015  
**Batch:** 1  
**Semester:** 5  
**Programme:** M.Sc Integrated in Data Science

## Project files
- `calculator.py` — Python addition function.
- `test_calculator.py` — three automated unit tests using Python's built-in `unittest`.
- `.github/workflows/ci.yml` — GitHub Actions workflow that runs tests on every push.

## Run locally
Open a terminal in this folder and run:

```bash
python calculator.py
python -m unittest -v
```

Expected result: all three tests pass.

## Test CI on GitHub
1. Create a GitHub repository named `CI_Experiment`.
2. Upload all files and folders in this project. Keep `.github/workflows/ci.yml` at exactly that path.
3. Open the repository's **Actions** tab and select **Python CI** to see the run.
4. To demonstrate a failure, temporarily change `return a + b` to `return a - b` in `calculator.py`, commit/push, and inspect the failed run.
5. Restore `return a + b`, commit/push again, and verify all tests pass.

GitHub Actions screenshots will only be available after you push the project to your own GitHub repository. The ZIP does not contain fabricated live GitHub results.
