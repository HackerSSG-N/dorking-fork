# For password

### Usage org:uber (below dork)
```bash
password= NOT password=(password) NOT password=(value) NOT password=(val) NOT password=(plain_text) NOT password=(unencrypted_password) NOT -password=<value>   NOT password={password} NOT password=${password} NOT /ADMIN_PASSWORD="password"/ NOT PASSWORD=# NOT /PASSWORD=${password}/   NOT password=(new_password) NOT /PASSWORD="$INPUT_PASSWORD"/ NOT /PASSWORD="$INPUT_APP_PASSWORD"/ NOT PASSWORD='password' NOT /PASSWORD="${ADMIN_PASSWORD:-password}"/ NOT /password=${env:SSL_KEYSTORE_PASSWORD}/ NOT password='" NOT password=' '  NOT Password=password  NOT password=%s NOT PASSWORD=$ NOT PASSWORD="***INVALID***" NOT PASSWORD="$ NOT password=<password> NOT TEST_GITHUB_PASSWORD= NOT password=" NOT password=secret</code> NOT password=options.password NOT user=%u&password=%p NOT PASSWORD=<your-password-here> NOT password=%v NOT PASSWORD=<admin-password> NOT password=\fR\fB\fIpassword\fR\fR NOT password=mypassword NOT password=\fR  NOT PASSWORD=.  NOT password=qwerty  
```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# For Github Token

### Usage org:uber (below dork)
```
GITHUB_TOKEN= OR GH_TOKEN= NOT GH_TOKEN='token' NOT GH_TOKEN=<secret token> NOT GH_TOKEN="<github token>" NOT GH_TOKEN="<USER_GITHUB_TOKEN>" NOT GH_TOKEN="<YOUR-GITHUB-API-TOKEN>" NOT GH_TOKEN="<your_github_access_token>" NOT GH_TOKEN=<MY_GITHUB_TOKEN>" NOT GH_TOKEN=<your_github_token> NOT GH_TOKEN="<unecrypted token>" NOT GH_TOKEN="<access_token>" NOT GH_TOKEN=<copied token> NOT GH_TOKEN=<personal github token>" NOT GH_TOKEN=xxxxxxx NOT GH_TOKEN="<Your Personal Access Token> NOT GH_TOKEN="<TOKEN>" NOT GH_TOKEN=<token> NOT GH_TOKEN=<YOUR TOKEN> NOT GH_TOKEN=<github token> NOT GH_TOKEN=<<TOKEN>>
```
