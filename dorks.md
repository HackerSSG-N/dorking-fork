# 1-For password

```bash
(password= OR SECRET= OR TOKEN= OR passwd= OR KEY=) NOT (password=(password) NOT password=(value) NOT password=(val) NOT password=(plain_text) NOT password=(unencrypted_password) NOT -password=<value>   NOT password={password} NOT password=${password} NOT /ADMIN_PASSWORD="password"/ NOT PASSWORD=# NOT /PASSWORD=${password}/   NOT password=(new_password) NOT /PASSWORD="$INPUT_PASSWORD"/ NOT /PASSWORD="$INPUT_APP_PASSWORD"/ NOT PASSWORD='password' NOT /PASSWORD="${ADMIN_PASSWORD:-password}"/ NOT /password=${env:SSL_KEYSTORE_PASSWORD}/ NOT password='" NOT password=' '  NOT Password=password  NOT password=%s NOT PASSWORD=$ NOT PASSWORD="***INVALID***" NOT PASSWORD="$ NOT password=<password> NOT TEST_GITHUB_PASSWORD= NOT password=" NOT password=secret</code> NOT password=options.password NOT user=%u&password=%p NOT PASSWORD=<your-password-here> NOT password=%v NOT PASSWORD=<admin-password> NOT password=qwerty ) 
```
For SSH Keys
```bash
org:shopify (SSH_PRIVATE_KEY= OR SSH_PUBLIC_KEY= OR id_rsa= OR id_dsa= OR id_ed25519= OR known_hosts= OR .ssh/id_rsa= OR .ssh/id_dsa= OR .ssh/id_ed25519= OR .ssh/config= OR .ssh/authorized_keys= OR .ssh/known_hosts=)
```



-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
