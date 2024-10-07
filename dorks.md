# 1-For password

```bash
(password= OR SECRET= OR TOKEN= OR passwd= OR KEY=) NOT (password=(password) NOT password=(value) NOT password=(val) NOT password=(plain_text) NOT password=(unencrypted_password) NOT -password=<value>   NOT password={password} NOT password=${password} NOT /ADMIN_PASSWORD="password"/ NOT PASSWORD=# NOT /PASSWORD=${password}/   NOT password=(new_password) NOT /PASSWORD="$INPUT_PASSWORD"/ NOT /PASSWORD="$INPUT_APP_PASSWORD"/ NOT PASSWORD='password' NOT /PASSWORD="${ADMIN_PASSWORD:-password}"/ NOT /password=${env:SSL_KEYSTORE_PASSWORD}/ NOT password='" NOT password=' '  NOT Password=password  NOT password=%s NOT PASSWORD=$ NOT PASSWORD="***INVALID***" NOT PASSWORD="$ NOT password=<password> NOT TEST_GITHUB_PASSWORD= NOT password=" NOT password=secret</code> NOT password=options.password NOT user=%u&password=%p NOT PASSWORD=<your-password-here> NOT password=%v NOT PASSWORD=<admin-password> NOT password=qwerty ) 
```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 3-For API Key
```bash
(API_KEY= OR API_SECRET= OR API_TOKEN= OR API_AUTH_KEY= OR API_ACCESS_KEY= OR API_ACCESS_TOKEN= OR API_SECRET_KEY= OR API_AUTH_TOKEN= OR API_CLIENT_KEY= OR API_CLIENT_SECRET= OR API_CREDENTIALS= OR API_PRIVATE_KEY= OR API_PUBLIC_KEY= OR API_SECURITY_KEY= OR API_SECURITY_TOKEN= OR API_ENCRYPTION_KEY= OR API_APP_KEY= OR API_APP_SECRET= OR API_KEY_SECRET= OR API_OAUTH_TOKEN= OR API_BEARER_TOKEN= OR API_SIGNING_KEY= OR API_AUTHORIZATION_TOKEN= OR API_MASTER_KEY=) NOT (API_KEY=<Your> OR API_SECRET={Your app API Secret} OR API_SECRET_KEY OR API_KEY=... OR api_key=(api_key) OR API_KEY=${withAPIKey} OR API_SECRET=YOUR_SHOPIFY_SECRET OR API_KEY=YOUR_SHOPIFY_API_KEY OR API_KEY=$ OR API_KEY=<Your Shopify API key> OR API_KEY=<your-api-key> OR api_key=your_api_key OR API_KEY=test-api-key OR API_SECRET=test-secret-key OR api_key=\"YOUR API KEY\")
```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 6-For SSH Keys
```bash
org:shopify (SSH_PRIVATE_KEY= OR SSH_PUBLIC_KEY= OR id_rsa= OR id_dsa= OR id_ed25519= OR known_hosts= OR .ssh/id_rsa= OR .ssh/id_dsa= OR .ssh/id_ed25519= OR .ssh/config= OR .ssh/authorized_keys= OR .ssh/known_hosts=)
```



-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
