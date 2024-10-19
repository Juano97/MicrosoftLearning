# Cryptography

## Concepts Learned

### Basics of Encryption

#### Different types of encryptions
There are several different types of symmetric and asymmetric encryption, and new versions are being invented all the time. Here are some that you may encounter:

> `Data Encryption Standard (DES) and Triple-DES.` This was one of the first symmetric encryption standards used.

> `Advanced encryption standard (AES).` AES replaced DES and Triple DES, and is still widely used today.

> `RSA.` This was one of the first asymmetric encryption standards, and variations are still being used today.

### Hashing and its Application in Digital Signing

A digital signature will always be unique to each person signing a document, much like one that's been handwritten. All digital signatures use an asymmetric key pair: the private and public keys.

Using a digital signing service, Monica can assign a digital signature to the document to prove that it hasn’t changed. Signing the document creates a time-stamped hash for it. This hash is then encrypted using Monica’s private key. Next, the signing service appends the hash to the original document, which isn't encrypted. Finally, both the digitally signed document and Monica’s public key are sent to Victoria.

When Victoria receives the digitally signed document, she uses the same digital signing service to extract Monica’s hash from the document, and generate a fresh hash for the original plaintext document. Then, using Monica’s public key, the encrypted hash is decrypted. If Monica’s decrypted hash matches the one Victoria created for the document, then the digital signature is valid. Victoria then knows that the document hasn’t been tampered with.

