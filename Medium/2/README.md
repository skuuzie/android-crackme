*10000% native code security*

<details>
  <summary>Hints</summary>

- only AES and RSA is used
- i used openssl, if that helps
- logcat
- again, should you really reverse the entire decryption flow just to get the flag?
</details>

<details>
  <summary>Stuck?</summary>

- aes_ecb(rsa_pkcs1_oaep_decrypt(encrypted_aes_key), encrypted_flag)
- Try to match/guess which openssl function is which, once you get it, you just have to intercept the decryption in action - no need for complete reversal
</details>