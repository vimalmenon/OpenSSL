# OpenSSL


--- 
### openssl
Openssl version with all detail (Can also be used without -a)
```bash
openssl version -a
```
Openssl shows all 
```bash
openssl version --help
```
Openssl help 
```bash
openssl help
```
Checking sha456 of a file 
```bash
sha256sum <filename>
```
Checking sha456 of a file using openssl
```bash
openssl sha256 <filename>
```
Putting sha456 of a file to <output-file-name>
```bash
openssl sha256 - hex -out <output-file-name> <filename>
```
Create symmetric key with byte <number>
```bash
openssl rand -hex <number>
```
Create symmetric key with byte <number> output to <output-file-name>
```bash
openssl rand -hex -out <output-file-name <number>
```
Generate asymmetric key with size (Size is optional)
```bash
openssl genrsa <size>
```
Generate asymmetric key put to <output-file-name>
```bash
openssl genrsa -out <output-file-name>
```
Check if the generated key with filename
```bash
openssl genrsa -in <output-file-name> -noout -text
```
Create public key of private key
```bash
openssl rsa -in <private-key> -pubout -out <public-key-file>
```
List all the command to encrypt the data
```bash
openssl list -commands
```
List all the digest algorithms
```bash
openssl list -digest-algorithms
```
List all the cipher algorithms
```bash
openssl list -cipher-algorithms
```

* Notes
  - 5 pillars of Cryptography
    - integrity
    - confidentiality
    - Authentication
    - Authorization
    - Non repudiation
--- 
