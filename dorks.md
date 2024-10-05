# 1-For password

### Usage org:uber (below dork)
```bash
password= NOT password=(password) NOT password=(value) NOT password=(val) NOT password=(plain_text) NOT password=(unencrypted_password) NOT -password=<value>   NOT password={password} NOT password=${password} NOT /ADMIN_PASSWORD="password"/ NOT PASSWORD=# NOT /PASSWORD=${password}/   NOT password=(new_password) NOT /PASSWORD="$INPUT_PASSWORD"/ NOT /PASSWORD="$INPUT_APP_PASSWORD"/ NOT PASSWORD='password' NOT /PASSWORD="${ADMIN_PASSWORD:-password}"/ NOT /password=${env:SSL_KEYSTORE_PASSWORD}/ NOT password='" NOT password=' '  NOT Password=password  NOT password=%s NOT PASSWORD=$ NOT PASSWORD="***INVALID***" NOT PASSWORD="$ NOT password=<password> NOT TEST_GITHUB_PASSWORD= NOT password=" NOT password=secret</code> NOT password=options.password NOT user=%u&password=%p NOT PASSWORD=<your-password-here> NOT password=%v NOT PASSWORD=<admin-password> NOT password=\fR\fB\fIpassword\fR\fR NOT password=mypassword NOT password=\fR  NOT PASSWORD=.  NOT password=qwerty  
```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 2-For Github Token

### Usage org:uber (below dork)
## Normal
```
(GITHUB_TOKEN= OR GH_TOKEN= OR GITHUB_ACCESS_TOKEN= OR GITHUB_API_TOKEN= OR GH_ACCESS_TOKEN= OR GH_API_TOKEN= OR GITHUB_SECRET= OR GH_SECRET= OR GITHUB_PERSONAL_ACCESS_TOKEN= OR GH_PERSONAL_ACCESS_TOKEN= OR GITHUB_OAUTH_TOKEN= OR GH_OAUTH_TOKEN= OR GITHUB_APP_TOKEN= OR GH_APP_TOKEN= OR GITHUB_CREDENTIALS= OR GH_CREDENTIALS= OR GITHUB_TOKEN_SECRET= OR GH_TOKEN_SECRET=)
```
## With Not operator
```
(GITHUB_TOKEN= OR GH_TOKEN= OR GITHUB_ACCESS_TOKEN= OR GITHUB_API_TOKEN= OR GH_ACCESS_TOKEN= OR GH_API_TOKEN= OR GITHUB_SECRET= OR GH_SECRET= OR GITHUB_PERSONAL_ACCESS_TOKEN= OR GH_PERSONAL_ACCESS_TOKEN= OR GITHUB_OAUTH_TOKEN= OR GH_OAUTH_TOKEN= OR GITHUB_APP_TOKEN= OR GH_APP_TOKEN= OR GITHUB_CREDENTIALS= OR GH_CREDENTIALS= OR GITHUB_TOKEN_SECRET= OR GH_TOKEN_SECRET=) NOT (GH_TOKEN='token' OR GH_TOKEN=<secret token> OR GH_TOKEN="<github token>" OR GH_TOKEN="<USER_GITHUB_TOKEN>" OR GH_TOKEN="<YOUR-GITHUB-API-TOKEN>" OR GH_TOKEN="<your_github_access_token>" OR GH_TOKEN=<MY_GITHUB_TOKEN> OR GH_TOKEN=<your_github_token> OR GH_TOKEN="<unecrypted token>" OR GH_TOKEN="<access_token>" OR GH_TOKEN=<copied token> OR GH_TOKEN=<personal github token> OR GH_TOKEN=xxxxxxx OR GH_TOKEN="<Your Personal Access Token>" OR GH_TOKEN="<TOKEN>" OR GH_TOKEN=<token> OR GH_TOKEN=<YOUR TOKEN> OR GH_TOKEN=<github token> OR GH_TOKEN=<<TOKEN>>)
```

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 3-For API Key
```bash
(API_KEY= OR API_SECRET= OR API_TOKEN= OR API_AUTH_KEY= OR API_ACCESS_KEY= OR API_ACCESS_TOKEN= OR API_SECRET_KEY= OR API_AUTH_TOKEN= OR API_CLIENT_KEY= OR API_CLIENT_SECRET= OR API_CREDENTIALS= OR API_PRIVATE_KEY= OR API_PUBLIC_KEY= OR API_SECURITY_KEY= OR API_SECURITY_TOKEN= OR API_ENCRYPTION_KEY= OR API_APP_KEY= OR API_APP_SECRET= OR API_KEY_SECRET= OR API_OAUTH_TOKEN= OR API_BEARER_TOKEN= OR API_SIGNING_KEY= OR API_AUTHORIZATION_TOKEN= OR API_MASTER_KEY=) NOT (API_KEY=<Your> OR API_SECRET={Your app API Secret} OR API_SECRET_KEY OR API_KEY=... OR api_key=(api_key) OR API_KEY=${withAPIKey} OR API_SECRET=YOUR_SHOPIFY_SECRET OR API_KEY=YOUR_SHOPIFY_API_KEY OR API_KEY=$ OR API_KEY=<Your Shopify API key> OR API_KEY=<your-api-key> OR api_key=your_api_key OR API_KEY=test-api-key OR API_SECRET=test-secret-key OR api_key=\"YOUR API KEY\")
```
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 4-For AWS Keys
```bash
(AWS_ACCESS_KEY_ID= OR AWS_SECRET_ACCESS_KEY= OR AWS_SESSION_TOKEN= OR AWS_SECURITY_TOKEN= OR AWS_SECRET_KEY= OR AWS_KEY= OR aws_access_key_id= OR aws_secret_access_key= OR aws_session_token= OR aws_key=)  NOT (AWS_ACCESS_KEY_ID=<Your AWS Access Key ID> OR AWS_SECRET_ACCESS_KEY=<Your AWS Secret Access Key> OR aws_access_key_id=EXAMPLE OR aws_secret_access_key=EXAMPLE OR AWS_ACCESS_KEY_ID=your_access_key OR AWS_SECRET_ACCESS_KEY=your_secret_key OR aws_access_key_id=\"YOUR_AWS_ACCESS_KEY_ID\" OR aws_secret_access_key=\"YOUR_AWS_SECRET_ACCESS_KEY\" OR aws_access_key_id=test OR aws_secret_access_key=test OR AWS_ACCESS_KEY_ID=<aws-access-key> OR AWS_SECRET_ACCESS_KEY=<aws-secret-access-key> OR AWS_ACCESS_KEY_ID="<s3_key>" OR AWS_SECRET_ACCESS_KEY="<s3_secret_key>" OR  aws_access_key="aws_access_key" OR aws_secret_key="aws_secret_key"
)
```
