# Create Private key and Public key in MacOS

## 1. Install `openssl`
```
brew install openssl
```

## 2. Check `openssl` 
```
openssl version
```

## 3. Create private key
```
openssl genrsa \                     
-out rsa-private-key.pem \
2048
```

## 4. Create public key from private key
```
openssl rsa -in rsa-private-key.pem \
-pubout \
-outform PEM \
-out rsa-public-key.pem
```
