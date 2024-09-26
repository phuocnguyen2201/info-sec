
# ONE-WAY FUNCTIONS
- One-way functions are easy to execute, encrypt (compute) and it is hard to reverse back to original form.
- We can take Lego as an example, it is easy to put pieces into a whole complete figure with instruciton paper, but when you tear it down and do it again without the instruction that would be really hard, and not fun anymore. (Only your imagination could help you now)
# ONE-WAY HASH FUNCTIONS
- Some other names: compression function, contraction function, message digest, fingerprint, cryptographic checksum, message integrity check (MIC), and manipulation detection code (MDC).
- The main function is to take the string input (**Pre-image**) and convert it into a fixed length of string(**Hash value**).
- Example: we're all have seen last lession, easy to turn some clear text into hash, or some type of encryptions but it is super hard or impossible to reverse.
## Message Authentication Codes
- MAC, the hash value depends on both the pre-image and the key. It's similar to hash functions, but only those with the key can verify it. A MAC can be created from a hash function, block cipher, or as a dedicated algorithm.
## How can one-way functions apply? 
- I have a login function and MD5 for hashing.
- I Create new user with the hashed password store in the database.
- How the program know to verify correctly the password? Decryption the password everytime when user logining? that would take a lot of their time, so no.
- The program simply just very the previous hashed stored password with the hashing when user trying to logining, same hashing same ciphertext, then the program can verify it.

## a/ Install Hashcat
## PROBLEMS
- Can't find the hashcat, the apt-get update command keep return 404

![alt Not Found](image/h6/notfound.PNG)

- Succeed to install from github, but another problem taking place which is the limitation of VirtualBox, its can't fully access the hardware.

![alt Hardware problem](image/h6/hardware-problem.PNG)

- The only option that available is windows. The password is **summer**

![alt result cracking password](image/h6/result.PNG)

## b/ Crack this hash: d595b2086532422bbe654bc07ea030df

- ## NOTES: I CAN'T INSTALL HASHCAT ON DEBIAN.
- ## MANAGED TO INSTALL FROM GITHUB BUT THE VIRTUALBOX CAN'T FULLY ACCESS TO HARDWARE (GPU) SO IT CAN'T CRACKING THE HASH. SO I COMBINED TOOL THAT WORK ON BOTH OS.

- Identify the hash type. (Let's just choose md5 with mode is 0)

![alt identify the hash](image/h6/identify.PNG)

- The crack command 

![alt Command](image/h6/command.PNG)

- The result (The red underline is the hash code and the password), password is **disobey**

![alt Result](image/h6/infomation.PNG)

## m/ Compile John the Ripper, Jumbo version

- Installation process

![alt configuration command](image/h6/configuration.png)

- Compilation

![alt compilation process](image/h6/compilation.png)

- Check the scriptes provided by John the Ripper

![alt scripts from john the ripper](image/h6/check-the-scripts.png)

- Test run.

![alt a test run](image/h6/start-up-the-machine.png)

## n/ Crack a zip file password

- Create a zip file with password using 7zip (you can see the password in the command, but let's just pretend you don't know it)

![alt Result](image/h6/zip-with-password.png)

- Create hash file

![alt create hash file](image/h6/hash-the-zip-file.png)

- Cracking the file's password, you can see the password is in **orange**.

![alt cracking the file's password](image/h6/cracking-the-second-password.png)

## o/ Crack a pdf password

- Create pdf hash file with **pdf2john.pl**.

![alt create the hash file](image/h6/create-hash-pdf.PNG)

- Check the hash file if the format is correct.

![alt check the hash file format](image/h6/check-hash-file.PNG)

- And the result.

![alt the result](image/h6/the-result.PNG)

- Open the file.

![alt open the file](image/h6/final-view.PNG)

# Reference

- https://terokarvinen.com/information-security/#h6-september2024
- https://terokarvinen.com/2023/crack-file-password-with-john/
- https://terokarvinen.com/2022/cracking-passwords-with-hashcat/
- https://github.com/benjamin-awd/pdf2john/blob/main/README.md
- https://infosecscout.com/install-hashcat-on-windows/