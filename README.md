# ECE444-Lab6
Sepehr Tahmasebi

--

## Pro 1: Creates a safety net for when code is refactored and changed
Properly implemented TDD can prevent code from failing when it is being refactored or changed, much better than regular unit tests would. Tests on important features can ensure that typical user actions (eg. logging in) are still functional when even minor changes are made, to ensure the user experience is protected when code is being iterated upon (eg. might be helpful where code is continuously being updated, such as a startup).

## Pro 2: Forces elements of code to be more independent and modular
Elements of an application are forced to be more separate, otherwise tests are hard to construct (as a single test would be testing multiple application components, which would be inconvenient -- there is usually a one-one relationship in tests where a single test will test a single application feature).

## Con 1: Tests need to be updated as the codebase changes
Since tests are not completely independent of the code they are testing, if the application structure changes significantly, the dependencies of the tests can mean that TDD adds a significant amount of time to development when the original code is changed.

## Con 2: Tests may take a long time to write and may not be easy to devise
In environments where code need to be implemented quickly (eg. startups), TDD may not be appropriate as the priority is to get features out, rather than for them to be perfect and error-free. As with unit tests, coming up with the right types of errors to test may not be easy, and writing the tests themselves can be as time consuming as writing the original code that need to be implemented.