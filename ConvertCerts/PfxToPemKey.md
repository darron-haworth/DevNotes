# Convert PFX to PEM and KEY

Question: How do I convert my .pfx file to .pem and .key files?

Answer:

The output will end up being the following two files:

1) Server.key : the private key associated with the certificate
2) Cert.pem :  the public SSL certificate

Using Open SSL, you can extract the certificate and private key.

To extract the private key from a .pfx file, run the following OpenSSL command:

openssl pkcs12 -in cert.pfx -nocerts -out pk.pem

The private key that you have extracted will be encrypted, to unencrypt the file so that it can be used, 
you want to run the following command:

```
openssl rsa -in pk.pem -out Server.key
```

To get the corresponding Server Certificate, you will run the following OpenSSL command:

```
openssl pkcs12 -in cert.pfx -clcerts -nokeys -out Cert.pem
```
