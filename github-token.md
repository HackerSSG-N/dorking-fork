# For Github Token
# Overview of GitHub Token Credential Dork

This GitHub dork is designed to search for repositories that may inadvertently expose sensitive GitHub authentication tokens and API keys. These tokens are crucial for accessing GitHub APIs and services securely, and their exposure can lead to unauthorized access to accounts and repositories.

## Key Parameters

The dork targets a variety of GitHub-related authentication tokens, including:

- **General Tokens**:
  - `GITHUB_TOKEN`
  - `GH_TOKEN`
  - `GITHUB_ACCESS_TOKEN`
  - `GITHUB_API_TOKEN`
  - `GH_ACCESS_TOKEN`
  - `GH_API_TOKEN`
  - `GITHUB_SECRET`
  - `GH_SECRET`
  - `GITHUB_PERSONAL_ACCESS_TOKEN`
  - `GH_PERSONAL_ACCESS_TOKEN`
  
- **OAuth Tokens**:
  - `GITHUB_OAUTH_TOKEN`
  - `GH_OAUTH_TOKEN`
  
- **App Tokens**:
  - `GITHUB_APP_TOKEN`
  - `GH_APP_TOKEN`
  
- **Credentials**:
  - `GITHUB_CREDENTIALS`
  - `GH_CREDENTIALS`
  - `GITHUB_TOKEN_SECRET`
  - `GH_TOKEN_SECRET`
  
- **API Keys**:
  - `GITHUB_API_KEY`
  - `GH_API_KEY`
  
- **Client Secrets**:
  - `GITHUB_CLIENT_SECRET`
  - `GH_CLIENT_SECRET`
  
- **Session Tokens**:
  - `GITHUB_SESSION_TOKEN`
  - `GH_SESSION_TOKEN`
  
- **Service Tokens**:
  - `GITHUB_SERVICE_TOKEN`
  - `GH_SERVICE_TOKEN`
  
- **Access Keys**:
  - `GITHUB_ACCESS_KEY`
  - `GH_ACCESS_KEY`

## Purpose

The primary purpose of this dork is to identify repositories where developers may have accidentally committed sensitive authentication tokens and keys. Exposing these credentials can allow attackers to gain unauthorized access to GitHub accounts and repositories, potentially leading to data breaches or malicious activities.

## Usage

To use this dork effectively:
1. Enter the dork into the GitHub search bar.
2. Review the search results for repositories that may contain exposed tokens and credentials.
3. Follow ethical guidelines and responsible disclosure practices if you identify any exposed tokens.

## Conclusion

This GitHub dork serves as a valuable tool for security researchers and developers to uncover potential vulnerabilities related to authentication tokens. Proper management of these credentials is vital for maintaining the security of GitHub accounts and repositories.


### ==>Simple one

```bash
(GITHUB_TOKEN=ghp_ OR  GH_TOKEN=ghp_ OR  GITHUB_ACCESS_TOKEN=ghp_ OR  GITHUB_API_TOKEN=ghp_ OR  GH_ACCESS_TOKEN=ghp_ OR  GH_API_TOKEN=ghp_ OR  GITHUB_SECRET=ghp_ OR  GH_SECRET=ghp_ OR  GITHUB_PERSONAL_ACCESS_TOKEN=ghp_ OR  GH_PERSONAL_ACCESS_TOKEN=ghp_ OR  GITHUB_OAUTH_TOKEN=ghp_ OR  GH_OAUTH_TOKEN=ghp_  OR  GITHUB_API_KEY=ghp_ OR  GH_API_KEY=ghp_  OR  GITHUB_ACCESS_KEY=ghp_ OR  GH_ACCESS_KEY=ghp_ OR GITHUB_PAT=ghp_ OR GH_PAT=ghp_ OR GITHUB_USER_TOKEN=ghp_ OR  GITHUB_PRIVATE_TOKEN=ghp_ OR GH_AUTH_TOKEN=ghp_ OR GITHUB_AUTH_TOKEN=ghp_ OR GITHUB_KEY=ghp_ OR GITHUB_APP_ID=ghp_ OR gH_auth_token=ghp_ OR GITHUB_AUTH=ghp_ OR github_refresh_token=ghp_ OR GITHUB_RUNNER_TOKEN=ghp_ OR GITHUB_AUTH_KEY=ghp_ OR REACT_APP_GITHUB_AUTHORIZATION_CODE=ghp_) AND (=ghp_f OR =ghp_g OR =ghp_h OR =ghp_i)
```

### ==>Give Specific ghp_ results

```bash
(GITHUB_TOKEN=ghp_ OR  GH_TOKEN=ghp_ OR  GITHUB_ACCESS_TOKEN=ghp_ OR  GITHUB_API_TOKEN=ghp_ OR  GH_ACCESS_TOKEN=ghp_ OR  GH_API_TOKEN=ghp_ OR  GITHUB_SECRET=ghp_ OR  GH_SECRET=ghp_ OR  GITHUB_PERSONAL_ACCESS_TOKEN=ghp_ OR  GH_PERSONAL_ACCESS_TOKEN=ghp_ OR  GITHUB_OAUTH_TOKEN=ghp_ OR  GH_OAUTH_TOKEN=ghp_ OR  GITHUB_APP_TOKEN=ghp_ OR  GH_APP_TOKEN=ghp_ OR  GITHUB_CREDENTIALS=ghp_ OR  GH_CREDENTIALS=ghp_ OR  GITHUB_TOKEN_SECRET=ghp_ OR  GH_TOKEN_SECRET=ghp_ OR  GITHUB_API_KEY=ghp_ OR  GH_API_KEY=ghp_ OR  GITHUB_CLIENT_SECRET=ghp_ OR  GH_CLIENT_SECRET=ghp_ OR  GITHUB_SESSION_TOKEN=ghp_ OR  GH_SESSION_TOKEN=ghp_ OR  GITHUB_SERVICE_TOKEN=ghp_ OR  GH_SERVICE_TOKEN=ghp_ OR  GITHUB_ACCESS_KEY=ghp_ OR  GH_ACCESS_KEY=ghp_)
```

### ==>Give Specific gho_ results

```bash
(GITHUB_TOKEN=gho_ OR  GH_TOKEN=gho_ OR  GITHUB_ACCESS_TOKEN=gho_ OR  GITHUB_API_TOKEN=gho_ OR  GH_ACCESS_TOKEN=gho_ OR  GH_API_TOKEN=gho_ OR  GITHUB_SECRET=gho_ OR  GH_SECRET=gho_ OR  GITHUB_PERSONAL_ACCESS_TOKEN=gho_ OR  GH_PERSONAL_ACCESS_TOKEN=gho_ OR  GITHUB_OAUTH_TOKEN=gho_ OR  GH_OAUTH_TOKEN=gho_ OR  GITHUB_APP_TOKEN=gho_ OR  GH_APP_TOKEN=gho_ OR  GITHUB_CREDENTIALS=gho_ OR  GH_CREDENTIALS=gho_ OR  GITHUB_TOKEN_SECRET=gho_ OR  GH_TOKEN_SECRET=gho_ OR  GITHUB_API_KEY=gho_ OR  GH_API_KEY=gho_ OR  GITHUB_CLIENT_SECRET=gho_ OR  GH_CLIENT_SECRET=gho_ OR  GITHUB_SESSION_TOKEN=gho_ OR  GH_SESSION_TOKEN=gho_ OR  GITHUB_SERVICE_TOKEN=gho_ OR  GH_SERVICE_TOKEN=gho_ OR  GITHUB_ACCESS_KEY=gho_ OR  GH_ACCESS_KEY=gho_)
```

### ==>Give Specific ghu_ results

```bash
(GITHUB_TOKEN=ghu_ OR  GH_TOKEN=ghu_ OR  GITHUB_ACCESS_TOKEN=ghu_ OR  GITHUB_API_TOKEN=ghu_ OR  GH_ACCESS_TOKEN=ghu_ OR  GH_API_TOKEN=ghu_ OR  GITHUB_SECRET=ghu_ OR  GH_SECRET=ghu_ OR  GITHUB_PERSONAL_ACCESS_TOKEN=ghu_ OR  GH_PERSONAL_ACCESS_TOKEN=ghu_ OR  GITHUB_OAUTH_TOKEN=ghu_ OR  GH_OAUTH_TOKEN=ghu_ OR  GITHUB_APP_TOKEN=ghu_ OR  GH_APP_TOKEN=ghu_ OR  GITHUB_CREDENTIALS=ghu_ OR  GH_CREDENTIALS=ghu_ OR  GITHUB_TOKEN_SECRET=ghu_ OR  GH_TOKEN_SECRET=ghu_ OR  GITHUB_API_KEY=ghu_ OR  GH_API_KEY=ghu_ OR  GITHUB_CLIENT_SECRET=ghu_ OR  GH_CLIENT_SECRET=ghu_ OR  GITHUB_SESSION_TOKEN=ghu_ OR  GH_SESSION_TOKEN=ghu_ OR  GITHUB_SERVICE_TOKEN=ghu_ OR  GH_SERVICE_TOKEN=ghu_ OR  GITHUB_ACCESS_KEY=ghu_ OR  GH_ACCESS_KEY=ghu_)
```


### ==>Give Specific ghs_ results

```bash
(GITHUB_TOKEN=ghs_ OR  GH_TOKEN=ghs_ OR  GITHUB_ACCESS_TOKEN=ghs_ OR  GITHUB_API_TOKEN=ghs_ OR  GH_ACCESS_TOKEN=ghs_ OR  GH_API_TOKEN=ghs_ OR  GITHUB_SECRET=ghs_ OR  GH_SECRET=ghs_ OR  GITHUB_PERSONAL_ACCESS_TOKEN=ghs_ OR  GH_PERSONAL_ACCESS_TOKEN=ghs_ OR  GITHUB_OAUTH_TOKEN=ghs_ OR  GH_OAUTH_TOKEN=ghs_ OR  GITHUB_APP_TOKEN=ghs_ OR  GH_APP_TOKEN=ghs_ OR  GITHUB_CREDENTIALS=ghs_ OR  GH_CREDENTIALS=ghs_ OR  GITHUB_TOKEN_SECRET=ghs_ OR  GH_TOKEN_SECRET=ghs_ OR  GITHUB_API_KEY=ghs_ OR  GH_API_KEY=ghs_ OR  GITHUB_CLIENT_SECRET=ghs_ OR  GH_CLIENT_SECRET=ghs_ OR  GITHUB_SESSION_TOKEN=ghs_ OR  GH_SESSION_TOKEN=ghs_ OR  GITHUB_SERVICE_TOKEN=ghs_ OR  GH_SERVICE_TOKEN=ghs_ OR  GITHUB_ACCESS_KEY=ghs_ OR  GH_ACCESS_KEY=ghs_)
```



### ==>With NOT Operator
```bash
(GITHUB_TOKEN= OR GH_TOKEN= OR GITHUB_ACCESS_TOKEN= OR GITHUB_API_TOKEN= OR GH_ACCESS_TOKEN= OR GH_API_TOKEN= OR GITHUB_SECRET= OR GH_SECRET= OR GITHUB_PERSONAL_ACCESS_TOKEN= OR GH_PERSONAL_ACCESS_TOKEN= OR GITHUB_OAUTH_TOKEN= OR GH_OAUTH_TOKEN= OR GITHUB_APP_TOKEN= OR GH_APP_TOKEN= OR GITHUB_CREDENTIALS= OR GH_CREDENTIALS= OR GITHUB_TOKEN_SECRET= OR GH_TOKEN_SECRET=) NOT (GH_TOKEN='token' OR GH_TOKEN=<secret token> OR GH_TOKEN="<github token>" OR GH_TOKEN="<USER_GITHUB_TOKEN>" OR GH_TOKEN="<YOUR-GITHUB-API-TOKEN>" OR GH_TOKEN="<your_github_access_token>" OR GH_TOKEN=<MY_GITHUB_TOKEN> OR GH_TOKEN=<your_github_token> OR GH_TOKEN="<unecrypted token>" OR GH_TOKEN="<access_token>" OR GH_TOKEN=<copied token> OR GH_TOKEN=<personal github token> OR GH_TOKEN=xxxxxxx OR GH_TOKEN="<Your Personal Access Token>" OR GH_TOKEN="<TOKEN>" OR GH_TOKEN=<token> OR GH_TOKEN=<YOUR TOKEN> OR GH_TOKEN=<github token> OR GH_TOKEN=<<TOKEN>>)
```


# If found valid so verify and report

```console
curl -H "Authorization: token GHSAT0AAAAAACUBHYZWBY2ELCUDSV7VBFY4ZUHTKRA" -H "Accept: application/vnd.github.v3+json" https://api.github.com/user



curl --request GET \
--url "https://api.github.com/user" \
--header "Authorization: Bearer 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" \
--header "X-GitHub-Api-Version: 2022-11-28"



curl --request GET \
--url "https://api.github.com/user/repos?visibility=private" \
--header "Authorization: Bearer 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" \
--header "X-GitHub-Api-Version: 2022-11-28"



curl --request GET \
--url "https://api.github.com/user/repos?visibility=all" \
--header "Authorization: Bearer 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" \
--header "X-GitHub-Api-Version: 2022-11-28"
```
