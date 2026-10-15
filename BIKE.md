# BIKE: Bit Flipping Key Encapsulation

**1. Family:**      
             BIKE belongs to the code-based post-quantum cryptography (PQC) family. It is based on the computational difficulty of decoding certain error-correcting codes, particularly quasi-cyclic moderate-density parity-check (QC-MDPC) codes. Unlike RSA and Diffie–Hellman, its security does not rely on integer factorization or discrete logarithms.  

**2. Type:**   
           BIKE is a public-key Key Encapsulation Mechanism (KEM). A KEM enables two parties to establish a shared secret over a public communication channel.
           
           It consists of three principal algorithms:
           
           KeyGen: Generates a public key and a private key.
           Encaps: Uses the recipient's public key to generate a ciphertext and a shared secret.
           Decaps: Uses the recipient's private key and the ciphertext to recover the shared secret. /

The shared secret can then be used with a symmetric encryption algorithm to protect application data.

**3. Subtype:**  
BIKE is a code-based, quasi-cyclic KEM based on QC-MDPC codes. It uses structured binary polynomials and an error-correction process to recover secret information.

Its construction also incorporates cryptographic transformations intended to provide security against chosen-ciphertext attacks (CCA), including a Fujisaki–Okamoto-style transform in the submitted design. 

**4. Other / Common Names:**
              
             1. BIKE
             2. Bit Flipping Key Encapsulation
             3. BIKE KEM
             4. QC-MDPC-based Key Encapsulation Mechanism
BIKE is the official algorithm name used in the NIST post-quantum cryptography evaluation process. 

**5. Purpose:**  
The primary purpose of BIKE is to establish a cryptographic shared secret in a way designed to remain secure against attackers with quantum-computing capabilities.

  Its intended uses include:

     > Establishing session keys for secure communication.
     > Supporting hybrid key establishment during migration to post-quantum cryptography.
     > Providing an alternative security foundation to lattice-based KEMs.
     > Protecting the key-establishment stage of protocols that subsequently use symmetric encryption.

BIKE was designed as an alternative to other post-quantum KEMs, with relatively compact public keys and ciphertexts compared with some code-based alternatives. However, BIKE was not selected by NIST for standardization in the fourth round. 

