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
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 5-For DATABASE Keys
```bash
(DATABASE_HOST= OR DATABASE_NAME= OR DATABASE_PASSWORD= OR DATABASE_PORT= OR DATABASE_USER= OR DATABASE_USERNAME= OR databaseEnabled= OR datadog_api_key= OR datadog_app_key= OR DB_CONNECTION= OR DB_DATABASE= OR DB_HOST= OR DB_PASSWORD= OR DB_PORT= OR DB_PW= OR DB_USER= OR DB_USERNAME= OR MONGO_URI= OR MONGODB_URI= OR MYSQL_HOST= OR MYSQL_USER= OR MYSQL_PASSWORD= OR MYSQL_DATABASE= OR POSTGRES_HOST= OR POSTGRES_USER= OR POSTGRES_PASSWORD= OR POSTGRES_DB= OR SQL_SERVER= OR SQL_USER= OR SQL_PASSWORD= OR SQL_DATABASE= OR SQL_HOST= OR RDS_HOSTNAME= OR RDS_DB_NAME= OR RDS_USERNAME= OR RDS_PASSWORD= OR REDIS_HOST= OR REDIS_PASSWORD= OR REDIS_PORT= OR oracle_host= OR oracle_user= OR oracle_password= OR oracle_sid= OR CASSANDRA_USERNAME= OR CASSANDRA_PASSWORD= OR elasticsearch_host= OR elasticsearch_username= OR elasticsearch_password= OR DB2_DATABASE= OR DB2_USER= OR DB2_PASSWORD=) 
```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 6-For SSH Keys
```bash
org:shopify (SSH_PRIVATE_KEY= OR SSH_PUBLIC_KEY= OR id_rsa= OR id_dsa= OR id_ed25519= OR known_hosts= OR .ssh/id_rsa= OR .ssh/id_dsa= OR .ssh/id_ed25519= OR .ssh/config= OR .ssh/authorized_keys= OR .ssh/known_hosts=)
```

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 7-For Payment Processor
```bash
(STRIPE_SECRET_KEY= OR STRIPE_API_KEY= OR STRIPE_CLIENT_SECRET= OR STRIPE_ACCESS_TOKEN= OR STRIPE_PUBLIC_KEY= OR PAYPAL_CLIENT_ID= OR PAYPAL_SECRET= OR PAYPAL_API_KEY= OR PAYPAL_ACCESS_TOKEN= OR BRAINTRREE_ACCESS_TOKEN= OR BRAINTRREE_MERCHANT_ID= OR BRAINTRREE_PUBLIC_KEY= OR BRAINTRREE_PRIVATE_KEY=)
```


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 8-Communication Channel
```bash
(STRIPE_SECRET_KEY= OR STRIPE_API_KEY= OR STRIPE_CLIENT_SECRET= OR STRIPE_ACCESS_TOKEN= OR STRIPE_PUBLIC_KEY= OR PAYPAL_CLIENT_ID= OR PAYPAL_SECRET= OR PAYPAL_API_KEY= OR PAYPAL_ACCESS_TOKEN= OR BRAINTRREE_ACCESS_TOKEN= OR BRAINTRREE_MERCHANT_ID= OR BRAINTRREE_PUBLIC_KEY= OR BRAINTRREE_PRIVATE_KEY=)
```



-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
