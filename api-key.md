# Overview of API Credentials GitHub Dork

This GitHub dork is designed to search for exposed API credentials across public repositories on GitHub. API credentials are essential for accessing various web services securely, and their exposure can lead to unauthorized access and potential misuse.

## Key Parameters

The dork targets a variety of API-related credential parameters, including:

- **General API Credentials**:
  - `API_KEY`
  - `API_SECRET`
  - `API_TOKEN`
  - `API_AUTH_KEY`
  - `API_ACCESS_KEY`
  - `API_ACCESS_TOKEN`
  - `API_SECRET_KEY`
  - `API_AUTH_TOKEN`
  - `API_CLIENT_KEY`
  - `API_CLIENT_SECRET`
  - `API_CREDENTIALS`
  - `API_PRIVATE_KEY`
  - `API_PUBLIC_KEY`
  - `API_SECURITY_KEY`
  - `API_SECURITY_TOKEN`
  - `API_ENCRYPTION_KEY`
  - `API_APP_KEY`
  - `API_APP_SECRET`
  - `API_KEY_SECRET`
  - `API_OAUTH_TOKEN`
  - `API_BEARER_TOKEN`
  - `API_SIGNING_KEY`
  - `API_AUTHORIZATION_TOKEN`
  - `API_MASTER_KEY`

## Exclusions

To avoid retrieving false positives, the dork specifically excludes results that match common placeholder or example values, such as:

- `API_KEY=<Your>`
- `API_SECRET={Your app API Secret}`
- `API_SECRET_KEY`
- `API_KEY=...`
- `api_key=(api_key)`
- `API_KEY=${withAPIKey}`
- `API_SECRET=YOUR_SHOPIFY_SECRET`
- `API_KEY=YOUR_SHOPIFY_API_KEY`
- `API_KEY=$`
- `API_KEY=<Your Shopify API key>`
- `API_KEY=<your-api-key>`
- `api_key=your_api_key`
- `API_KEY=test-api-key`
- `API_SECRET=test-secret-key`
- `api_key="YOUR API KEY"`

## Purpose

The primary goal of this dork is to uncover repositories where developers might have accidentally committed sensitive API credentials. Unauthorized access to APIs can result in data breaches, account takeovers, and potential financial losses for both users and service providers.

## Usage

To use this dork effectively:
1. Input the dork into the GitHub search bar.
2. Review the search results for any repositories containing exposed API credentials.
3. Follow ethical practices and responsible disclosure if any sensitive information is discovered.

## Conclusion

This GitHub dork is a valuable tool for security researchers, developers, and organizations aiming to identify and rectify the exposure of sensitive API credentials in public repositories. Proper management and safeguarding of API keys and secrets are crucial to maintaining security in application development and deployment.



```bash
(API_KEY= OR API_SECRET= OR API_TOKEN= OR API_AUTH_KEY= OR API_ACCESS_KEY= OR API_ACCESS_TOKEN= OR API_SECRET_KEY= OR API_AUTH_TOKEN= OR API_CLIENT_KEY= OR API_CLIENT_SECRET= OR API_CREDENTIALS= OR API_PRIVATE_KEY= OR API_PUBLIC_KEY= OR API_SECURITY_KEY= OR API_SECURITY_TOKEN= OR API_ENCRYPTION_KEY= OR API_APP_KEY= OR API_APP_SECRET= OR API_KEY_SECRET= OR API_OAUTH_TOKEN= OR API_BEARER_TOKEN= OR API_SIGNING_KEY= OR API_AUTHORIZATION_TOKEN= OR API_MASTER_KEY=) NOT (API_KEY=<Your> OR API_SECRET={Your app API Secret} OR API_SECRET_KEY OR API_KEY=... OR api_key=(api_key) OR API_KEY=${withAPIKey} OR API_SECRET=YOUR_SHOPIFY_SECRET OR API_KEY=YOUR_SHOPIFY_API_KEY OR API_KEY=$ OR API_KEY=<Your Shopify API key> OR API_KEY=<your-api-key> OR api_key=your_api_key OR API_KEY=test-api-key OR API_SECRET=test-secret-key OR api_key=\"YOUR API KEY\")
```
