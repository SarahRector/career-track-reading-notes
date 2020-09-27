# Why you should use BCrypt to hash passwords
https://medium.com/@danboterhoven/why-you-should-use-bcrypt-to-hash-passwords-af330100b861

* encryption solutions are often not solid enough. Even with attaching random strings to passwords, hackers can still gain access to your data

* BCrypt uses block cipher cryptomatic algorithms in an adaptive  hash function
  * basically it slows down the speed at which hashing happens, which means the amount of time it would take to crack the password usually isn't worth it

# Hashing in Action: Understanding bcrypt
https://auth0.com/blog/hashing-in-action-understanding-bcrypt/

* so users put in their plaintext passwords and then they need to be hashed. Hashing by itself isn't good enough so then we need to add a salt to the end of the hash (random info)

* bcrypt hashes and salts at the same time

* what even is a rainbow table?

* example of bcrypt in node.js:
```js
const bcrypt = require("bcrypt");
const plainTextPassword1 = "DFGh5546*%^__90";

for (let saltRounds = 10; saltRounds < 21; saltRounds++) {
  console.time(`bcrypt | cost: ${saltRounds}, time to hash`);
  bcrypt.hashSync(plainTextPassword1, saltRounds);
  console.timeEnd(`bcrypt | cost: ${saltRounds}, time to hash`);
}
```
* two factor authentication means that a hacker couldn't just crack a password. They would need to crack the password and the random code on top of the password

# Token Storage
https://auth0.com/docs/tokens/token-storage

* making sure tokens and API calls are secure

* good resource page for info about auth in different scenarios