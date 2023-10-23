
Marshalling - packing parameters into a message

Unmarshalling - unpacking parameters from a message

Marshalling & unmarshalling involves wrapping a parameter which means transforming a value into a sequence of bytes (known as Serialisation)

	Serialisation - a data structure/object state that needs to be translated into a format that can be stored (e.g. file/memory data buffer) or transmitted

The client and server have to agree on the same encoding so they need to properly interpret messages and transform them into machine-dependent representations

2 questions asked when marshalling data:

- How are basic data values represented? (i.e. integers, floats, characters etc)
- How are complex data values represented? (i.e. arrays, unions etc)

Data marshalling issues:

- Client and server might encode characters differently
- Client and server might implement integers and floating-point numbers dig