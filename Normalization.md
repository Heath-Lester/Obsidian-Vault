https://en.wikipedia.org/wiki/Database_normalization

Database normalization is the process of structuring a relational database in accordance with a series of so-called normal forms to reduce redundancy and improve data integrity.

Normal Forms:

1. Unique rows (no duplicate records)
2. Scalar columns (columns cannot contain relations for composite values)
3. Every Non-prime attribute has a full functional dependency on a candidate key
4. Every non-trivial functional dependency either begins with a superkey or ends with a prime attribute
5. Every non-trivial functional dependency either begins with a superkey or ends with an elementary prime attribute
6. Every non-trivial functional dependency begins with a superkey
7. Every non-trivial multivalued dependency begins with a superkey
8. Every join dependency has a superkey component
9. Every constraint is a consequence of domain constraints and key constraints
10. Every join dependency is trivial