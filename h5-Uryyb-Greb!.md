

# € Schneier 2015: Applied Cryptography

1. ## Foundation.

- **Messages, Encryption and Decryption**
    The purpose is to disguise the message. The process turn clear text to ciphertext called **Encryption**, a disguised message is called **ciphertext**, the opposite of **Encryption** is **Decryption** which is turn ciphertext back to clear text.

- **Authentication, Integrity, and Nonrepudiation**
    - Authentication: the receiver must have a valid credential to access to message.
    - Integrity: the message have not modified during the transmit process, and the original of the text is still remain.
    - Nonrepudiation: A sender should not be able to falsely deny later that he sent a message.

- **Algorithms and Keys**
    - A cryptographic algorithm is using for encryption or decryption.
    - Key could be random of anything (text, numbers) could be use in encryption and decryption operation.
    - A cryptosystem is combined plaintexts, ciphertexts and keys.

- **Symmetric Algorithms**
    Most symmetric algoritms, the encryption and decryption key are the same.

- **Public-Key Algorithms**
    Designed so the key for encryption could be different to decryption.

- **Cryptanalysis**
    Cryptanalysis is recovering ciphertext back to clear text without a valid key.

- **Security of Algorithms**
    Nothing is absolutely, so the algorithms. Any Algorithm could be breakthoughs in cryptanalysis, but the important that your data is still secure at some level.

- **Computer Algorithms**
    Three main cryptographic algorithms:
        - DES (Data Encryption Standard) is the most popular computer encryption algorithm
        - RSA (named for its creators—Rivest, Shamir, and Adleman) is the most popular public-key algorithm
        - DSA (Digital Signature Algorithm, used as part of the Digital Signature Standard) is another public-key algorithm



2. ## CRYPTOGRAPHIC PROTOCOLS.

- Protocal is a set of steps, that we must follow to achieve something. Moreover, it must be done in the right order.
- **Basic protocals** is encrypt each of individual conversation with separate key, they trade for each other and using it only for communication.

3. ## PGP - Send Encrypted and Signed Message - gpg

    - Installing it by using the command **sudo apt-get install gpg micro psmisc**
    - Create a keypari using **gpg --gen-key**, and the program asking in order to enter name, email and secret phrases.
    - We are done with the first person, export to send to the trusted person.
    - We do the same for the second person.
    - We import the key from the first person
    - Sign it with sign-key


* ## a. Encrypt and decrypt with GNUPG


* ## o. Frequency distribution of letters for a language

- According to google, the letters N, H and C are the most frequent letters in the Vietnamese language.

- 6 most frequently are **N, H, C ,T, I, G**

* ## p. Install OpenSSH server, connect to it using 'ssh' client.

- Check server status.

![alt SSH Server status](image/ssh-server-status.png)


- Connect using SSH.

![alt Connect using ssh](image/connect-via-ssh.png)
