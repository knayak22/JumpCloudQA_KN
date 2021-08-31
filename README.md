I used the windows version of password had program when I first started this. 

After multiple attempts to get this to work using the commands mentioned in the assignment document, I found that it is not applicable when run using Windows OS. When running in Windows, curl does not recognize single quotes. Double quotes needs to be used instead. In this case in the json we would need to use escape characters but it was not working either. So ended up using a json.txt format to send as password input in the POST to /hash request. So most of my screenshots from my tests were using the .txt file as json input

Various inputs used when testing password hash
json1.txt
{"password": "angrymonkey"}

json2.txt
{"password": "testing"}

json3.txt
{"password": "AngryMonkey"}

json4.txt
{"pwd": "angrymonkey"}

json5.txt
{"password": ""}

json6.txt
{"password": "@ngrym0nkey"}

json7.txt
{"password": "12345"}

I downloaded Git for Windows which has a Git BASH, a BASH emulation in windows environment. In this environment the curl commands worked as provided in the assignment. When I ran the Post commands here, I saw that it also provided the timings of how long the processing time was. 

Other important links used:
- Get the SHA512 hash value of the password provided
https://www.dcode.fr/sha512-hash
https://passwordsgenerator.net/sha512-hash-generator/
https://sha512.online/ 

- Get the base64 encoded password for the SHA512 hashed value
https://emn178.github.io/online-tools/base64_encode.html 

The Jumpcloud-assignment.docx includes the following details on the assignment:

- Application Details
- Requirements
- Table of Test case Summary
- Test case execution with details and screenshots of results
- Bug summary
