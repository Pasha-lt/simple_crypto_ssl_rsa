# simple_crypto_ssl_rsa
* echo текст который я буду шифровать > tekst.txt 
* ssh-keygen -f cryptokey.pub -e -m PKCS8 > cryptokey.public
* openssl rsautl -encrypt -pubin -inkey cryptokey.public -in tekst.txt -out EncryptedMessage.txt
* openssl rsautl -decrypt -inkey cryptokey.private -in EncryptedMessage.txt -out Decryptor.txt
