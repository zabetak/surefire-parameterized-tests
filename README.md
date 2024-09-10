# surefire-parameterized-tests

The project demonstrates the usage of maven-surefire-plugin with include/exclude files and Junit parameterized tests.

```
mvn test -Dsurefire.includesFile=includes.txt
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.github.zabetak.TestClass2
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.037 s - in com.github.zabetak.TestClass2
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0
```

```
mvn test -Dsurefire.excludesFile=excludes.txt
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.github.zabetak.TestClass1
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.028 s - in com.github.zabetak.TestClass1
[INFO] Running com.github.zabetak.TestClass2
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.001 s - in com.github.zabetak.TestClass2
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0
```

