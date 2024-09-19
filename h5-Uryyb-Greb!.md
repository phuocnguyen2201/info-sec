

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

- **Steganography**
    Steganography hides secret messages within other messages, making the secret’s existence inconspicuous. Modern techniques involve embedding secret bits in the least significant bits of graphic images, allowing hidden messages without noticeable changes to the image.

- **Substitution Cipher**
    Substitution Cipher is one in which each character in the plaintext is substituted for another character in the ciphertext. The receiver inverts the substitution on the ciphertext to recover the plaintext.
    
- **Transposition Cipher**
    In a transposition cipher, the plaintext characters are shuffled. In a columnar transposition, the message is written in rows and read vertically to create the ciphertext, and decrypted by reversing this process.

- **One-time pad**
    Invented in 1917, uses a set of random key letters for encryption, where each key is used only once to encrypt one character of the message. Both sender and receiver have identical pads, and after encryption or decryption, the used keys are destroyed to ensure security.

2. ## CRYPTOGRAPHIC PROTOCOLS.

- Protocal is a set of steps, that we must follow to achieve something. Moreover, it must be done in the right order.
- **Basic protocals** is encrypt each of individual conversation with separate key, they trade for each other and using it only for communication.

* ## a. Encrypt and decrypt with GNUPG
    The concept is easy to understand, but when come to practice, I messed it up so many times, anyway I managed to done it:

    - Let gen the key from the first person.

    ![alt First Key](image/gen-key-first-person.png)

    - Export the key.

    ![alt Export the key](image/export-the-first-key.png)

    - Simulate the second person

    ![alt Simulate a fake second person](image/simulate-second-person.png)

    - Send the first key for second person

    ![alt Send the first key for second person](image/import-the-key-and-verify.png)

    - Verify and sign the key.

    ![alt Verify and sign the key](image/after-sign-the-key.png)

    - Now it turn for second person to do previous thing.

    ![alt Gen key from the second person](image/gen-key-second-person.png)

    - Export the key.

    ![alt Export the key](image/export-the-key-from-the-second-person.png)

    - Sign the second key.

    ![alt sign the second key](image/sign-the-second-key.png)

    - **Done!!!! you are secured, now it time for send the message**

    - Encypte the message, and see how it look like when encrypted.

    ![alt Encrypt the message](image/encrypt-the-message-and-verify-encrypted.png)

    - Simulate send the message to first person and decrypt it.

    ![alt Descrypt the message](image/decrypt-the-message.png)
* ## b. Password Manager

    **Keypass** - no cloud, open source, easy to use.

    - Start up screen. The software devide, credential into 5 different section, like General, Windows, Network, Internet, Email and Homebanking. Right now, i'm gonna focus on Internet because we're all surf alot on it. 

    ![alt Start-up the program](image/ui.PNG)

    - Adding the entry.

    ![alt Adding the entry](image/addentry.PNG)

    - Perform entering the credential.
    **IMPORTANT!!! MAKE YOU POINT TO THE RIGHT USERNAME FIELD FIRST, OR ELSE THE AUTO FULL FEATURE WILL PERFORM AT THE WRONG PLACE (Mine was the tool search the entire password on google)**

    [![Watch the video]](https://youtu.be/56Bt6swV5I4)

* ## n. Voluntary bonus: send and receive encrypted message over email.

    - Send and encryption.
    ![alt Encrypt email](image/encrypt-email.png)

    - Receive.
    ![alt receive email](image/receive.png)

    - Decrypt with options.
    ![alt Options for decrypt](image/option-decrypt.png)

    - After Decrypt.
    ![alt The message](image/the-message.png)

* ## o. Frequency distribution of letters for a language

- According to google, the letters N, H and C are the most frequent letters in the Vietnamese language.

- 6 most frequently are **N, H, C ,T, I, G**

* ## p. Install OpenSSH server, connect to it using 'ssh' client.

- Check server status.

![alt SSH Server status](image/ssh-server-status.png)


- Connect using SSH.

![alt Connect using ssh](image/connect-via-ssh.png)
