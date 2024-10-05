# For password

### Usage org:uber (below dork)
```bash
password= NOT password=(password) NOT password=(value) NOT password=(val) NOT password=(plain_text) NOT password=(unencrypted_password) NOT -password=<value>   NOT password={password} NOT password=${password} NOT /ADMIN_PASSWORD="password"/ NOT PASSWORD=# NOT /PASSWORD=${password}/   NOT password=(new_password) NOT /PASSWORD="$INPUT_PASSWORD"/ NOT /PASSWORD="$INPUT_APP_PASSWORD"/ NOT PASSWORD='password' NOT /PASSWORD="${ADMIN_PASSWORD:-password}"/ NOT /password=${env:SSL_KEYSTORE_PASSWORD}/ NOT password='" NOT password=' '  NOT Password=password  NOT password=%s NOT PASSWORD=$ NOT PASSWORD="***INVALID***" NOT PASSWORD="$ NOT password=<password> NOT TEST_GITHUB_PASSWORD= NOT password=" NOT password=secret</code> NOT password=options.password NOT user=%u&password=%p NOT PASSWORD=<your-password-here> NOT password=%v NOT PASSWORD=<admin-password> NOT password=\fR\fB\fIpassword\fR\fR NOT password=mypassword NOT password=\fR  NOT PASSWORD=.  NOT password=qwerty  
```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# For Github Token

### Usage org:uber (below dork)
```
(GITHUB_TOKEN= OR GH_TOKEN= OR GITHUB_ACCESS_TOKEN= OR GITHUB_API_TOKEN= OR GH_ACCESS_TOKEN= OR GH_API_TOKEN= OR GITHUB_SECRET= OR GH_SECRET= OR GITHUB_PERSONAL_ACCESS_TOKEN= OR GH_PERSONAL_ACCESS_TOKEN= OR GITHUB_OAUTH_TOKEN= OR GH_OAUTH_TOKEN= OR GITHUB_APP_TOKEN= OR GH_APP_TOKEN= OR GITHUB_CREDENTIALS= OR GH_CREDENTIALS= OR GITHUB_TOKEN_SECRET= OR GH_TOKEN_SECRET=) NOT (GH_TOKEN='token' OR GH_TOKEN=<secret token> OR GH_TOKEN="<github token>" OR GH_TOKEN="<USER_GITHUB_TOKEN>" OR GH_TOKEN="<YOUR-GITHUB-API-TOKEN>" OR GH_TOKEN="<your_github_access_token>" OR GH_TOKEN=<MY_GITHUB_TOKEN> OR GH_TOKEN=<your_github_token> OR GH_TOKEN="<unecrypted token>" OR GH_TOKEN="<access_token>" OR GH_TOKEN=<copied token> OR GH_TOKEN=<personal github token> OR GH_TOKEN=xxxxxxx OR GH_TOKEN="<Your Personal Access Token>" OR GH_TOKEN="<TOKEN>" OR GH_TOKEN=<token> OR GH_TOKEN=<YOUR TOKEN> OR GH_TOKEN=<github token> OR GH_TOKEN=<<TOKEN>>)
```
