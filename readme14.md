Define the term “hashing”.

Hashing is a process in computing and cryptography where a mathematical algorithm, called a hash function, is used to transform any type of data, such as text, files, or passwords, into a fixed-size, scrambled sequence of characters known as a hash. The goal of hashing is to take any input, regardless of its size, and produce a unique and consistent output of a fixed length.




we used hashing algorithms in computing and cryptography include:

Message Digest (MDx) Algorithms: These algorithms produce a fixed-length hash value from input data. Some well-known MDx algorithms include:

MD5 (Message Digest 5): Produces a 128-bit (16-byte) hash value. While it was widely used in the past, it's no longer considered secure for critical applications due to vulnerabilities.
MD4 (Message Digest 4): An older algorithm that's considered even less secure than MD5.

Secure Hash Algorithms (SHA): These algorithms are designed for secure data hashing and are considered more robust. Examples include:

SHA-1 (Secure Hash Algorithm 1): Produces a 160-bit (20-byte) hash value. It was widely used but is now deprecated due to vulnerabilities.
SHA-2 Family: Includes multiple algorithms like SHA-224, SHA-256, SHA-384, and SHA-512, which produce hash values of varying lengths. SHA-256 is one of the most widely used and considered secure for various applications.

Explain to a non-technical friend what a hash function does to a password.

Hashing is like a magical blender for passwords, turning them into jumbles of letters and numbers that are always the same for the same password but can't be reversed to find the original. It's a way to secure passwords, so even if someone gets hold of the jumble, they can't figure out your password. Websites use this jumble to check if you've entered the correct password without actually storing your real password, keeping your login information safe.




What does it mean to ‘salt’ a password?

‘salt’ adds a very long string of bytes to the password. So even though a hacker might gain access to one-way hashed passwords, they should not be able to guess the ‘salt’ string. In theory, this is a great way to secure your data, but if a hacker has access to your source code, they will easily be able to find the ‘salt’ string for passwords.




What piece of information would a hacker need to access in order to find the ‘salt’ string for your passwords?

To find the ‘salt’ string for passwords, a hacker would need access to the source code of the application or system where the salt is defined. one way for a hacker to find the salt string is to gain access to the source code of the application or system that uses salted password hashing. If the salt is hard-coded in the source code, it becomes relatively easy for the hacker to identify it.







How does the Blowfish block cipher handle the increased computation speed of new computers?

The Blowfish block cipher handles the increased computation speed of new computers by allowing the adjustment of the computation cost parameter, often referred to as "log_rounds." This parameterization of the computation cost ensures that the algorithm can be made more resource-intensive as computers become faster. This approach effectively raises the cost of offline password cracking, making it more challenging for attackers with fast hardware to crack hashed passwords.

What are the issue with the two most commong password hashes for Java (“Java password hash” and “Java password encryption”)?

Relatively Slow Performance: Both "Java password hash" and "Java password encryption" methods exhibit relatively slow performance. This slowness can become problematic, especially in situations where a large number of authentication requests need to be processed concurrently. If not configured properly, it can potentially lead to denial of service (DoS) attacks, where an attacker overwhelms the system with login requests, causing it to become unresponsive.

bcrypt's Lack of Adaptation to Hardware Advancements: In the case of bcrypt, it does not adapt to advancements in hardware over time. While this may seem like a security advantage, it can also affect consistent login performance. As computer hardware becomes more powerful, bcrypt remains equally slow, which means that the time required for password hashing and verification may not be optimal. This can lead to slower login processes for users, negatively impacting the user experience.