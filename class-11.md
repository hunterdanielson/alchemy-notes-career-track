# Alchemy Reading Notes

## Class 11

### User modeling
- Lots of sensitive information is provided by the user that must be protected
- User models have data that should **Never** be sent to the client application

### Cryptography
- A science way to encode messages so that only a person with a correct key may read the message

### Hash algorithms
- Takes data and makes a hash that is difficult to reverse
- Same data makes the same hash
- Often one wants to store a hash password on their backend instead of the actual password

### Cypher algorithms
- Takes a piece of data and a key and makes encrypted data, it can be decrypted with the same key

### Basic authorization
- Common method for username and password in a request
- It uses base64 encoding, but not encryption