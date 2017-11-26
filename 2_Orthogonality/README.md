# Orthogonality

A measure of how independent different modules and classes in a system are.

1. Which is more orthogonal of the classes Split1 and Split2?
    - Split1 requires a stream reader and implements an extra method to read subsequent lines. As such, it is bringing along implementation details from the stream reader. In contrast, Split2 accepts only a string and does not need to know about how that string is generated. It doesn't need to allow for the IOException either. Split2 is more orthogonal.
2. Out of modeless or modal dialog boxes, which will lead to more orthogonal design?
    - Modeless dialog boxes don't need to know about state and so are inherently more orthogonal.
3. Is procedural or object oriented language more orthogonal?
    - Procedural requires a lot of change when dependent components are modified. Object oriented programming by contrast can inherit different behaviour and carry out behaviour without needing to know implmementation specifics. Eg. by programming to an interface. OOP is more orthogonal.

Note on **3** from the book - procedural language can be orthogonal if written correctly and object-oriented code and end up as a *meatballs* mess if implemented badly. It's a case of adhering to good practices (orthogonality, SOLID, etc).