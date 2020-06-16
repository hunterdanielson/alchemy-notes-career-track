# Alchemy Reading Notes

## Class 12

### Why you should use Bcrypt
- It is a adaptive hash function.
- It can adjust the cost of hashing
- It is especially resistant to rainbow table hacks

### Understanding Bcrypt
The bcrypt hashing function allows us to build a password security platform that scales with computation power and always hashes every password with a salt.
- It is a one way hash with added salt
- It slows down the hashing process so it would take hackers too long to attempt to hack the hash

### Token Storage
- If your app is using a sign in scenario that doesn't require API calls, only an ID Token is required. There is no need to store it. You can validate it and get the data from it that you required.
- If your app needs to call APIs on behalf of the user, Access Tokens and (optionally) Refresh Tokens are needed. These can be stored server-side or in a session cookie.
- They recommend using the Auth0 SPA SDK to handle token storage, session management
