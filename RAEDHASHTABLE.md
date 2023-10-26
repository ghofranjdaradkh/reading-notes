Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value.




Analogy: Student ID Cards and Library Barcodes

Imagine student ID cards and library book barcodes as an analogy for hashing in universities and libraries. In both cases, these unique identifiers (student ID and book barcode) serve as keys to efficiently access information about students and books.

hashing is applied to a university's student record system to efficiently manage and access student information using unique roll numbers as keys. This concept can be extended to various applications where objects need to be uniquely identified for efficient data retrieval.

vocabulary

Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.




Structure of Hashing:

Hash Code Determinism:

Hash codes must be deterministic, meaning their output is solely determined by their input. There should be no randomness in hash code generation.
The same key should consistently yield the same hash code, ensuring reliability in data retrieval.

Creating a Hash Table:

Hash tables are typically constructed from arrays. A common practice is to choose an array size, often 1024, which plays a crucial role in determining index placement for efficient data storage.
Once the array is created, a process is applied to convert the "key" into a numerical value, which serves as the index for data storage and retrieval.

Hashing Algorithm:

A hashing algorithm is used to convert keys into numeric values. An example of a simplistic hashing algorithm includes the following steps:
Sum or multiply all ASCII values of the key characters together.
Multiply the result by a prime number (e.g., 599).
Apply the modulo operation to find the remainder when dividing the result by the total array size.
The resulting index is used for inserting data into the array.










Methods:

get()

The get() method takes in a key, gets the Hash, and goes to the index location specified. 

has()

The has() method will accept a key, and return a bool on if that key exists inside the hashtable. 

keys()

The keys() method returns a collection (array) of unique hash keys.

hash()

The hash() method will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.




















