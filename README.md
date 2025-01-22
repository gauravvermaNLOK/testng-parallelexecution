# testng-parallelexecution

**This Project talks about**
1. **Parallel Test Execution** of all Tests in TestNG (Ref: https://medium.com/@gauravverma.career/parallel-execution-in-maven-project-using-testng-framework-71bafa2a3bfa)
2. **Consolidate multiple TestNG in single TestNG** file (Ref: https://medium.com/@gauravverma.career/testng-suite-file-consolidate-multiple-testng-files-into-a-single-suite-2293e89d173c)

**How to run:**
Go to directory where pom.xml is residing run command
   mvn test -mvn test -DtestngFilePath={name of TestNg XML file}

   1. For **Parallel Test Execution** of all test methods, use testng.xml file. Command is mvn test -DtestngFilePath=testng.xml
   2. For **running consolidated TestNG file**, use MasterTestNG.xml. Command is mvn test -DtestngFilePath=MasterTestNG.xml
      MasterTestNG.xml has multiple TestNG file inside it.
