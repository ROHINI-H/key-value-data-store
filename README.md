# key-value-data-store
Build a file-based key-value data store that supports the basic CRD (create, read, and delete) operations using Nodejs and Json
This data store is meant to be used as a local storage for one single process on one
laptop. The data store must be exposed as a library to clients that can instantiate a class and work
with the data store.
The data store will support the following functional requirements.
1. It can be initialized using an optional file path. If one is not provided, it will reliably
create itself in a reasonable location on the laptop.
2. A new key-value pair can be added to the data store using the Create operation. The key
is always a string - capped at 32chars. The value is always a JSON object - capped at
16KB.
3. If Create is invoked for an existing key, an appropriate error must be returned.
4. A Read operation on a key can be performed by providing the key, and receiving the
value in response, as a JSON object.
5. A Delete operation can be performed by providing the key.

The "app.js" file contains the nodejs code to accomplish the above task.
The "db.json" file is a data store where the key-value pair of data are present.
The output of these code is shown in "output" file.
