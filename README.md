# Jest acts like --preserve-symlinks

Try the following

```
npm install

# This should fail, because `b` cannot require `a`
node app/index.js

# This should succeed, because this is what the flag does
node --preserve-symlinks app/index.js

# Interestingly, this behaves like the second
npm test
```
