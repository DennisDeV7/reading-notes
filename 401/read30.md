# Hash Tables

## Vocabulary

- Hash table: a data structure that uses a dictionary to map keys to values and assigns it an index so it can be found quickly.
- Hash function: a function that creates a map of values associated with a set of data
- Hash: data returned by a hash function
- Collision: When a hash function assigns the same index number to more than one key. This error usually needs to be accounted for in the code
- Buckets: A term used to describe the actual data associated with the index that is tied to the key value.
- Separate chaining: A technique to handle collisions. Builds a linked list which links the key-value pairs of the collided items.
- Linear probing: Another technique to handle collisions. This method analyzes the array first and inserts the data into empty slots. This is typically less efficient than separate chaining.
