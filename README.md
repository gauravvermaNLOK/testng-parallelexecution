# testng-parallelexecution

**This Project talks about**
1. **Parallel Test Execution** of all Tests in TestNG (Ref: https://medium.com/@gauravverma.career/parallel-execution-in-maven-project-using-testng-framework-71bafa2a3bfa)
2. **Consolidate multiple TestNG in single TestNG** file (Ref: https://medium.com/@gauravverma.career/testng-suite-file-consolidate-multiple-testng-files-into-a-single-suite-2293e89d173c)
3. **Run multiple TestNG in parallel without consolidating in Single TestNG** (Ref: https://medium.com/@gauravverma.career/parallel-test-execution-execute-multiple-testng-in-simultaneously-in-one-go-fc193550117b)

**How to run:**
Go to directory where pom.xml is residing run command
   mvn test -mvn test -DtestngFilePath={name of TestNg XML file}

   1. For **Parallel Test Execution** of all test methods, use testng.xml file. Command is mvn test -DtestngFilePath=testng.xml
   2. For **running consolidated TestNG file**, use MasterTestNG.xml. Command is mvn test -DtestngFilePath=MasterTestNG.xml
      MasterTestNG.xml has multiple TestNG file inside it.
   3. To **run multiple TestNG files in parallel without consolidating in single file** use command mvn test -DtestngFilePath=<comma separated TestNG file names>
   e.g. mvn test -DtestngFilePath="Test Class1.xml",TestClass2.xml,TestClass3.xml,TestClass4.xml
***Note:**
1. There should not be any space between comma (,) and testng file name.
2. If there is space in testng file name then enclose it in double quote(“ ”).
e.g.

mvn test -DtestngFilePath="Test Class1.xml",TestClass2.xml,TestClass3.xml,TestClass4.xml
