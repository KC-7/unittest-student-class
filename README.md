# Python Testing Demonstration Mini Project

This repository contains a Python script `student.py` and its corresponding test script `test_students.py`.

## Introduction

The `student.py` file contains a `Student` class with various methods that can be used to create and manipulate instances of `Student` objects. The `test_students.py` file contains several test cases that ensure the `Student` class and its methods are working as expected.

## Dependencies

The following dependencies are required to run the test_students.py script:

- Python 3.x
- `unittest` module
- `requests` module

## Installation and Usage

1. Clone the repository to your local machine

2. Navigate to the project directory in the terminal

3. Run the following command to execute the test script:

    `python test_students.py`

## Test Driven Development (TDD)

The `test_students.py` script was created using a TDD approach. This means that tests were written before any code was written. The tests were used as a guide to determine what code needed to be implemented. Once the tests were written, the code was written and tested until all tests passed. This ensures that the code meets the expected behavior defined in the tests.

## Red Green Refactor (RGR)

The `TestStudent` class follows the RGR approach to testing, where each test is initially written to fail (the "Red" phase), then the code is implemented to pass the test (the "Green" phase), and finally, the code is refactored to improve its quality and readability (the "Refactor" phase). This helps to ensure that the code is both correct and maintainable, and that any changes made to the code do not break existing functionality.

## Mocking

The `test_course_schedule_success` and `test_course_schedule_failed` methods use mocking to simulate the behavior of the `requests.get` method without actually making an HTTP request. This is done using the `unittest.mock.patch` decorator, which replaces the original method with a mock object that can be configured to return specific values. This allows the tests to be run without requiring a network connection or depending on external services.

## Tests

### TestStudent Class

1. test_full_name
    - Tests the full_name method
    - Asserts that the full name returned by the method is equal to the expected full name.

2. test_email
    - Tests the email method
    - Asserts that the email returned by the method is equal to the expected email.

3. test_alert_santa
    - Tests the alert_santa method
    - Asserts that the naughty_list attribute is set to True after the method is called.

4. test_apply_extension
    - Tests the apply_extension method
    - Asserts that the end_date attribute is updated correctly after the method is called.

5. test_course_schedule_success
    - Tests the course_schedule method when the HTTP request is successful
    - Mocks the requests.get function to return a successful response
    - Asserts that the response returned by the method is equal to the expected response.

6. test_course_schedule_failed
    - Tests the course_schedule method when the HTTP request fails
    - Asserts that the response returned by the method is equal to the expected response.


## Credits

- This mini project was created by following a Code Institute Walkthrough Tutorial as part of their Full Stack Developer Course. 

- This README file was partially created by passing code into ChatGPT to create detailed documentation for future reference.
