[![Coverage Status](https://coveralls.io/repos/github/MrStudentuser/VIII---Deployment/badge.svg?branch=main)](https://coveralls.io/github/MrStudentuser/VIII---Deployment?branch=main)

# Student template (Modified)

## Purpose of this repository

This is a project template for students participating in Software Testing course
at LAB University of Applied Sciences.

The repository only contains the source code that is under testing, `package.json` skeleton
and LICENSE file.

Source code folder contains a separate license file that must **NOT** be removed under any circumstances!
Removing this license file directly violates terms and conditions of the software under testing.
Individuals who remove or modify the license file will also carry the consequences.

## Testing

This project includes a unit testing suite implemented using Vitest.

### Installing

npm install

### Running coverage locally

npm run coverage

### Coverage

Test coverage is measured using Vitest and reported via Coveralls.

### Continuous Integration

GitHub Actions is used to automatically run tests and generate coverage reports on each push.

### Issues found during testing

During testing, several issues were discovered in the library:

divide.js - incorrect division logic
clamp.js - incorrect boundary handling
chunk.js - overwrites chunks due to missing index increment
compact.js - skips first valid element
countBy.js - initializes counts incorrectly
camelCase.js - produces leading whitespace

These issues have been reported in the repository issue tracker.

### Production readiness

The following files were tested:
 - Array utilities
 - Collection utilities
 - String utilities
 - Type-check utilities
 - Object/path utilities

Based on the testing results, the library is not ready for use without implementing fixes, as multiple core functions are broken.
