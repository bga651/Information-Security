# Summarise Applied Cryptography Chapter 1 by Schneier

The first part of the first chapter provides an overview of the foundational concepts in cryptography. It begins by explaining the terminology, such as sender and receiver, messages, encryption (disguising a message), and decryption (revealing the message). Cryptography is defined as the practice of securing messages, while cryptanalysis is the art of breaking encrypted messages. Cryptology encompasses both cryptography and cryptanalysis.

The article introduces the use of plaintext (M or P) as the original message and ciphertext (C) as the encrypted form of the message. Authentication, integrity, and nonrepudiation are highlighted as additional requirements beyond confidentiality. Authentication ensures the message's origin, integrity verifies that the message has not been altered, and nonrepudiation prevents the sender from denying sending the message.

The importance of cryptographic keys (K) in modern cryptography is emphasized. Keys are used in encryption and decryption processes, ensuring that even if the algorithm is known, without the specific key, the message remains secure.

Two main types of cryptographic algorithms are discussed: symmetric and public-key algorithms. Symmetric algorithms use the same key for both encryption and decryption and require secure key distribution. Public-key algorithms use different keys for encryption and decryption, enhancing security and allowing the public distribution of encryption keys.

The article explains various types of cryptanalytic attacks, such as ciphertext-only, known-plaintext, chosen-plaintext, and adaptive-chosen-plaintext attacks. It also mentions other types of attacks like chosen-ciphertext and chosen-key attacks, as well as non-cryptanalytic methods like rubber-hose cryptanalysis (threats, blackmail, torture, etc.).

The importance of making algorithms and methods public for peer review is highlighted, as it helps identify and rectify vulnerabilities. The article concludes by discussing the security of algorithms, emphasizing that cryptographic systems must remain secure even in the face of evolving computing power. It notes that only a one-time pad is unconditionally secure, while other systems aim to be computationally secure by making attacks infeasible with available resources.

Finally, the article touches upon historical terms like "code" (dealing with linguistic units) and "cipher" (useful for any circumstance), distinguishing between them in the context of cryptography.

The following chapters discusses various topics related to cryptography and encryption techniques. Here is a summary of the key points:

1.2 Steganography:
Steganography is the art of concealing secret messages within other messages to keep the existence of the secret hidden. Methods of steganography include using invisible inks, tiny pin punctures on selected characters, minute differences between handwritten characters, and even hiding messages within graphic images by modifying the least significant bits of each byte.

1.3 Substitution Ciphers and Transposition Ciphers:
Before the computer era, cryptography relied on character-based algorithms. Substitution ciphers replace characters in the plaintext with other characters in the ciphertext, while transposition ciphers shuffle the order of characters. Substitution ciphers can be simple, homophonic, polygram, or polyalphabetic. Transposition ciphers rearrange characters in a predictable manner. While these classical ciphers are relatively easy to break, they formed the basis for early cryptography.

Rotor Machines:
Rotor machines were developed in the 1920s to automate encryption. They used rotors with arbitrary permutations of the alphabet to perform substitutions. By combining multiple rotors and shifting them, rotor machines increased security. The Enigma machine, used by the Germans in World War II, is a famous example.

1.4 Simple XOR:
Simple XOR encryption is a basic symmetric encryption method that uses the XOR operation to combine the plaintext with a key. However, it is not considered secure, as it can be easily broken using simple techniques, making it unsuitable for serious encryption needs.

1.5 One-Time Pads:
A one-time pad is a theoretically perfect encryption scheme that relies on a truly random and non-repeating key. Each key character is used only once to encrypt a corresponding character in the plaintext. It offers absolute security as long as the key remains secret and is never reused. However, practical limitations, such as key distribution and synchronization, make it challenging to implement.

1.6 Computer Algorithms:
Modern computer encryption algorithms include DES (Data Encryption Standard), a symmetric algorithm; RSA, a public-key algorithm used for encryption and digital signatures; and DSA (Digital Signature Algorithm), another public-key algorithm used solely for digital signatures. These algorithms are widely used in computer security.

1.7 Large Numbers:
The article provides order-of-magnitude estimates for various large numbers relevant to cryptography. These numbers serve as physical analogies to help readers grasp the scale and significance of cryptographic calculations.

Overall, the article provides an overview of historical and modern encryption techniques, highlighting their strengths and weaknesses.

### Reference https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/08_chap01.html#chap01-sec007

# Find out frequency distribution of letters for a language that you know (other than English). What are the six most common letters? 

English is the only alphabetic language I speak. Hence it's hard for me to find our frequent letters to use in other alphabetic language. But I'm studying Finnish now so that if I would guess in Finnish, first of all vowels are probably most common letters to use for example "a" "e" "i". And then "n" "k" "t"are other letters that seems quite often use in Finnish. But I don't speak Finnish so I have no confident in this at all.

Let's Google it what is the most frequent letters in Finnish :D

<img width="475" alt="Screenshot 2023-09-16 at 20 47 16" src="https://github.com/bga651/Information-Security/assets/114089466/6912bfad-d995-4898-9dc5-ddc8d31d0edf">

It shows:
"A" 12.22

"I" 10.82

"N" 8.83

"T" 8.75

"E" 7.97

"S" 7.86
My guess was not too bad :D

### Reference http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/finnish-letter-frequencies/

# I choose DashLane as the example of password manager

### What threats does it protect against
It's primarily helps protect against a range of cybersecurity threats by enhancing password security and overall online security practices. Here are some of the threats that Dashlane helps protect against:

1. Password Theft: Dashlane securely stores passwords and allows users to generate complex, unique passwords for each online account. This makes it much more difficult for attackers to steal or guess passwords.

2. Phishing: Dashlane can help users recognize phishing websites by autofilling login credentials only on legitimate sites that match stored records. This helps prevent users from entering their passwords on fake or malicious websites.

3. Credential Reuse: Dashlane encourages users to avoid reusing passwords across multiple sites. This practice helps protect against the domino effect that can occur if one account is breached and the same password is used for other accounts.

4. Data Breaches: Dashlane provides breach alerts, notifying users when their login credentials have been compromised in a data breach. Users can then change their passwords promptly.

5. Keyloggers: Dashlane's automatic form filling and password entry can help protect against keyloggers, as users don't need to type their passwords manually.

6. Secure Password Generation: Dashlane includes a password generator that can create strong, random passwords, reducing the likelihood of passwords being cracked through brute force or dictionary attacks.

7. Two-Factor Authentication (2FA): Dashlane supports 2FA, adding an extra layer of security to user accounts by requiring a second form of authentication beyond just a password.

8. Secure Notes and Personal Information: In addition to passwords, Dashlane securely stores sensitive information like credit card details and personal notes, protecting them from unauthorized access.

9. Device Security: Dashlane offers secure synchronization between devices while ensuring that stored data is encrypted and protected.

10. Password Changer: Some password managers, including Dashlane, offer a feature that can automatically change passwords for supported websites, further reducing the risk of compromised accounts.

11. Phishing Warnings: Dashlane can provide warnings if a user visits a potentially malicious website, helping them avoid falling victim to phishing attacks.

### What information is encrypted, what's not?
Encrypted Data:

Passwords: The core functionality of Dashlane is to securely store and manage passwords. All stored passwords are encrypted to ensure they remain confidential. This means that even Dashlane itself cannot access your passwords.

Credit Card Information: Dashlane allows users to store credit card details for autofill during online shopping. This information is encrypted to protect it from unauthorized access.

Personal Notes: Users can create personal notes and store sensitive information, such as security questions and answers, in Dashlane's secure notes. These notes are encrypted to maintain confidentiality.

Identity Information: Dashlane can store various personal details, such as name, address, and contact information, to assist with online form filling. This data is encrypted to prevent unauthorized access.

Secure File Storage: Some password managers, including Dashlane, offer secure file storage. Files uploaded to Dashlane, such as documents or images, are typically encrypted to protect their contents.

Not Encrypted:

Usernames and URLs: Usernames and website URLs are usually not encrypted because Dashlane needs to access this information for autofill and login purposes. However, the associated passwords are encrypted.

Master Password: The master password you use to access your Dashlane account is not stored by Dashlane. Instead, it is used to derive an encryption key locally on your device. This key is used to decrypt your stored data when you log in.

Security Challenge Questions: Some password managers allow users to set up security challenge questions to recover their account. The answers to these questions may not be encrypted to allow for account recovery.

Two-Factor Authentication (2FA) Codes: If you use 2FA with Dashlane, the one-time codes generated by your authentication app are not stored by Dashlane. They are typically stored locally on your device.



# ETAOIN. When asked to come up with encryption scheme in the class, almost everyone described a variation of a simple substitution chipher. As requested, now it's time to attack your own scheme! Crack this ciphertext:

I worte all my thoughts in the Word, here is the screen shot for this.
<img width="889" alt="Screenshot 2023-09-15 at 23 15 44" src="https://github.com/bga651/Information-Security/assets/114089466/76280698-2456-4e33-b00f-75272f4494da">


<img width="880" alt="Screenshot 2023-09-15 at 23 16 01" src="https://github.com/bga651/Information-Security/assets/114089466/581605ba-d0fd-4eff-92f7-f3045a6b0aa0">

# Encrypt and Decrypt a message
As teach was demostred in the class, we used PGP and in the PGP, we were suggested GNU Privacy Guard (GnuPG or GPG) which is a free and open-source software application used for encrypting and decrypting messages and files. Here are the basic steps to encrypt and decrypt a message using GnuPG:

Encrypting a Message:

Install GnuPG: If you don't already have GnuPG installed on your system, you can download and install it from the official GnuPG website.

Generate Your Key Pair: Before you can encrypt messages, you need a key pair: a public key for encryption and a private key for decryption. If you don't already have one, you can generate a key pair using the gpg --gen-key command. Follow the prompts to create your key pair.

Obtain the Recipient's Public Key: To encrypt a message for someone else, you need their public key. You can import their public key into your keyring using the gpg --import command.

Encrypt the Message: To encrypt your message, use the gpg --encrypt -r recipient@example.com command, where recipient@example.com is the email address associated with the recipient's public key. You can also use their key ID instead of the email address.

Enter Your Message: GnuPG will prompt you to enter the message you want to encrypt. Type or paste your message and press Enter.

Output and Save the Encrypted Message: GnuPG will generate the encrypted message and display it on the screen. You can redirect this output to a file using the > operator. 

Decrypting a Message:

Import Your Private Key: Make sure your private key is available in your keyring. You usually only need to do this once when you generate your key pair.

Decrypt the Message: To decrypt an encrypted message, use the gpg --decrypt command followed by the path to the encrypted message file. 

Enter Your Passphrase: GnuPG will prompt you to enter the passphrase associated with your private key. This passphrase is used to unlock your private key for decryption.

View or Save the Decrypted Message: After entering the correct passphrase, GnuPG will display the decrypted message on the screen. You can also redirect the output to a file if you want to save it:

Remember to keep your private key secure and never share it with anyone. Your private key is used to decrypt messages meant for you.



