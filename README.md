# log-analyzer

# how to run
gradlew -Pparams="c:\logfiles\mylogentries.json" bootRun
gradlew --tests *
gradlew -Pparams="output.json" runLogGenerator

# todos
*Checked in my test local hssqldb files so you can view the insert stmts etc
*Tested with large "Generated" file of 147MB... no issues.. You can use the above runLogGenerator target to generate whatever size file you want although need to change the batch count and batch size in the code.. sorry ;)
*Its possible to run both the generator and the analyzer at the same time in two different consoles (or one as a background process), working on the same never ending file.
*Todos... continue to add UT/IT coverage around algorithm as noted in Listener Test 
