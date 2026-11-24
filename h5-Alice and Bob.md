## Read and summarize

### 1. Schneier (2015) -- *Applied Cryptography*, Chapter 1: Foundations

#### Section 1.1 -- Terminology

1.  **Sender and Receiver:** A sender who sends a message and a receiver
    who receives it. An attacker may try to intercept the communication.
2.  **Plaintext:** The original readable message before encryption.
3.  **Encryption:** The process of converting plaintext into unreadable
    ciphertext to protect information.
4.  **Decryption:** Converting ciphertext back into its original
    readable form.
5.  **Algorithms:** Mathematical procedures used to encrypt and decrypt
    information.
6.  **Keys:** Information used by cryptographic algorithms to control
    encryption and decryption.
7.  **Symmetric Algorithms:** Use the same secret key for encryption and
    decryption. Both parties must securely share the key.
8.  **Public-Key Algorithms:** Use two related keys: a public key that
    can be shared and a private key that must remain secret.
9.  **Main Difference:** Symmetric encryption is generally faster, while
    public-key encryption makes secure key exchange easier.

### 2. Schneier (2015) -- *Applied Cryptography*, Chapter 2

#### Section 2.5 -- Communications Using Public-Key Cryptography

1.  Public-key cryptography allows two parties to communicate securely
    without sharing a secret key beforehand.
2.  Each user generates two keys: a public key and a private key.
3.  The sender uses the recipient's public key to encrypt the message.
4.  The recipient uses their private key to decrypt the encrypted
    message.
5.  Private keys must remain secret, while public keys can be
    distributed openly.
6.  Public keys should be verified to ensure they belong to the intended
    recipient.
7.  This approach protects message confidentiality and supports secure
    communication.
8.  Public-key cryptography can also support digital signatures for
    message authenticity and integrity.
9.  **Merkle Puzzles:** A key-exchange technique that allows two parties
    to establish a shared secret over an insecure communication channel
    by solving cryptographic puzzles.
10. **Security of Merkle Puzzles:** The legitimate parties can solve a
    selected puzzle with relatively little effort, while an attacker
    intercepting all puzzles must solve many of them, requiring
    significantly more computational effort.

### 3. Tero Karvinen (2023) -- [PGP: Send Encrypted and Signed Message -- GPG](https://terokarvinen.com/2023/pgp-encrypt-sign-verify/)

1.  PGP (Pretty Good Privacy) is a cryptographic system used to encrypt
    and digitally sign messages to ensure secure communication.
2.  GPG (GNU Privacy Guard) is a free tool that implements OpenPGP and
    allows users to encrypt, sign and verify messages.
3.  Users first generate their own public and private key pairs using
    the `gpg --gen-key` command.
4.  Public keys are exchanged between users, while private keys are kept
    secret and never shared.
5.  Before trusting an exchanged public key, users should verify its
    fingerprint to confirm its ownership.
6.  Users can sign each other's verified public keys to establish trust.
7.  To send a secure message, the sender encrypts it using the
    recipient's public key and digitally signs it using their own
    private key.
8.  The recipient decrypts the message using their private key and
    verifies the sender's signature using the sender's public key.
9.  GPG displays a "Good signature" message when the signature is valid,
    indicating that the signed message has not been modified since it
    was signed.

## a) Pubkey today

We all use WhatsApp regularly for our day-to-day communication. WhatsApp
uses a protocol which relies on public-key cryptography and symmetric
encryption to protect messages.

1.  Each user has cryptographic keys, including a public key and a
    private key.
2.  When a conversation is started, the sender's device obtains the
    recipient's public key material.
3.  The sender's device uses its private key and the recipient's public
    key material to participate in establishing shared encryption
    secrets.
4.  Both devices derive symmetric encryption keys for protecting
    messages.
5.  The sender's messages are encrypted on their device before being
    sent to WhatsApp's servers.
6.  The recipient's device uses its corresponding keys to decrypt and
    read the messages.

## b) Encrypt and decrypt a message

For this task, I chose the browser-based online tool
[CipherKit](https://cipherkit.app/tools/rsa-encrypt-decrypt/). CipherKit
uses RSA encryption with SHA-256, which are considered strong
cryptographic methods when implemented correctly. It performs encryption
and decryption directly in the browser, so messages and keys are not
sent to its server, which improves privacy.

### Step 1: Generate public and private keys

First I generated public and private keys from the link below. I kept
the key size at 2048 bits and SHA-256 as my hashing algorithm.

[CipherKit RSA Key Pair
Generator](https://cipherkit.app/tools/rsa-key-generator/)

<img width="975" height="626" alt="image" src="https://github.com/user-attachments/assets/b26fc22e-b78a-42a6-8204-80487a4e7203" />


### Step 2: Encrypt a message using public key

-   I opened the [CipherKit RSA Encrypt/Decrypt
    tool](https://cipherkit.app/tools/rsa-encrypt-decrypt/).
-   I copied the public key from the previous step and pasted it in the
    public key section, entered a message in the plaintext section and
    clicked the **Encrypt** button.
    
<img width="853" height="925" alt="image" src="https://github.com/user-attachments/assets/77d30a6e-d0ac-468b-936f-f62ea79d071e" />

    
-   The encrypted message was displayed in the ciphertext section.

<img width="864" height="838" alt="image" src="https://github.com/user-attachments/assets/fc3bd543-4187-419f-bfa1-c9604f266187" />

### Step 3: Decrypt the message using private key

-   For decrypting the message, I copied the private key and pasted it
    in the private key section of the same page.
-   Then I copied the ciphertext, pasted it in the ciphertext section
    and clicked the **Decrypt** button.
-   The output was my original plaintext before encryption.

<img width="975" height="509" alt="image" src="https://github.com/user-attachments/assets/9ced31fe-60c9-46c4-9150-08c80e7ad66b" />


## c) Password Management

For this part, I selected Bitwarden. I personally use this password
manager and have been using it for a few years.

### How to use it?

-   Visit [Bitwarden](https://bitwarden.com/) and create a free account.
-   Log in to your Bitwarden vault.
-   Click **Add item** and select **Login**.
-   Enter a website name, username and test password.
-   Use the password generator to create a strong, random password.
-   Save the login details in your vault.
-   Open the saved entry to demonstrate how passwords are stored and
    accessed.

### Attacks that take advantage of people not using password managers

-   Attackers use stolen passwords from one website to access accounts
    on other websites.
-   Attackers use automated tools to guess weak passwords.
-   Attackers try common passwords against many different accounts.
-   Attackers create fake websites or emails to trick users into
    revealing their passwords.
-   Passwords written on paper or saved in unprotected files can be
    stolen.
