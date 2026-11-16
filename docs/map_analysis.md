# Map Analysis Laboratory

## Core goal
Students must implement a dictionary-like `Map` structure that stores key-value pairs and supports lookup, insertion, deletion, and updates.

## Required operations
Students must implement the following behavior:

- insert a new key-value pair;
- reject duplicate keys;
- find whether a key exists;
- update an existing value;
- remove an existing key;
- retrieve a value by key;
- list keys and values;
- maintain sorted order if appropriate for the design.

## Analysis expectations
Students should discuss:

- average-case time complexity of insertion, lookup, and deletion;

Insertion is O(n log n) since the vector gets sorted after insertion
Lookup is O(n) because the findIndex() function uses linear searching.
Deletion is O(n) because once a element is deleted, it must shift left.

-best-case and worst-case behavior;

O(1) when key is at the beginning of the map
Worst case is when they key doesn't exist at all O(n)

- why duplicate-key handling matters;

To avoid values having the same keys.

- the difference between a search by key and scanning all entries;

FindIndex is used when by key and, scanning all entries

- trade-offs between sorted vectors and hash-based maps;

Searching takes O(n) but keep the vectors organized.
Hash maps use more space but provide O(1) lookup.

- memory overhead and performance of `keys()` and `values()`

O(n) space and time complexity.

## Big-O focus
Students should explain the Big-O of:

- `insert` O(n log n) | sorts
- `contains` O(n) | linear search
- `update` O(n) | searches
- `erase` O(n) | searches then shifts
- `at` O(n) | searches
- `keys` O(n) | copies all of the keys
- `values` O(n) | copies all the values

The expected design is a clear, well-explained mapping abstraction that makes trade-offs explicit.
