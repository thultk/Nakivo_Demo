How to set up and run the tests:
1. Open a terminal window then clone the project
2. cd folder you clone the project into
3. mvn clean install

Notes:
1. To get forgot password (security string), the default path of forgot_password.txt is located at
C:\Program Files\NAKIVO Backup & Replication (Already declared in \src\main\java\commons\GlobalConstants.java).
If there are some changes, just update the path accordingly.
2. The test cases TC_05_DynamicTesting, TC_06_ForgotPassword, TC_09_SecurityValidation_ValidEmailFormats and the rest of remaining
test cases should use different user accounts (Can add or modify user account here: 
\src\test\java\com\nakivo\data\User.java)
3. Update test suite or test class that you want to run here:
\src\test\resources\runNakivoTestcases.xml
4. In this release, only support run with chrome first
5. In this release, not yet supported print out customized reports

Questions:
Test case 4: Login form requires username instead of an email address. In reality, should clarify with BA/PO
for unclear cases like this. Just continue working to show how to handle these edge cases
