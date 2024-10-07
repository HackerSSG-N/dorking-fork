
# Overview of Password Credentials GitHub Dork

This GitHub dork is constructed to search for exposed password credentials within public repositories on GitHub. The accidental exposure of passwords can lead to unauthorized access and significant security vulnerabilities.

## Key Parameters

The dork targets various parameters associated with passwords, including:

- **Common Password Identifiers**:
  - `password=`
  - `SECRET=`
  - `TOKEN=`
  - `passwd=`
  - `KEY=`

## Exclusions

To filter out irrelevant results and avoid false positives, the dork excludes matches with the following conditions:

- `password=(password)`
- `password=(value)`
- `password=(val)`
- `password=(plain_text)`
- `password=(unencrypted_password)`
- `-password=<value>`
- `password={password}`
- `password=${password}`
- `/ADMIN_PASSWORD="password"/`
- `PASSWORD=#`
- `/PASSWORD=${password}/`
- `password=(new_password)`
- `/PASSWORD="$INPUT_PASSWORD"/`
- `/PASSWORD="$INPUT_APP_PASSWORD"/`
- `PASSWORD='password'`
- `/PASSWORD="${ADMIN_PASSWORD:-password}"/`
- `/password=${env:SSL_KEYSTORE_PASSWORD}/`
- `password='"`
- `password=' '`
- `Password=password`
- `password=%s`
- `PASSWORD=$`
- `PASSWORD="***INVALID***"`
- `PASSWORD="$`
- `password=<password>`
- `TEST_GITHUB_PASSWORD=`
- `password="`
- `password=secret`
- `password=options.password`
- `user=%u&password=%p`
- `PASSWORD=<your-password-here>`
- `password=%v`
- `PASSWORD=<admin-password>`
- `password=qwerty`

## Purpose

The primary aim of this dork is to identify repositories where developers may have inadvertently committed sensitive password information. Exposure of passwords can lead to data breaches, unauthorized account access, and other security incidents.

## Usage

To use this dork effectively:
1. Enter the dork into the GitHub search bar.
2. Carefully review the search results for any repositories that may contain exposed password credentials.
3. Adhere to responsible disclosure practices if any sensitive information is identified.

## Conclusion

This GitHub dork serves as a valuable tool for security researchers, developers, and organizations looking to find and mitigate the risk of exposed passwords in public repositories. Proper handling and safeguarding of passwords are essential to maintaining security in software development and operational environments.



```bash
(password= OR SECRET= OR TOKEN= OR passwd= OR KEY=) NOT (password=(password) NOT password=(value) NOT password=(val) NOT password=(plain_text) NOT password=(unencrypted_password) NOT -password=<value>   NOT password={password} NOT password=${password} NOT /ADMIN_PASSWORD="password"/ NOT PASSWORD=# NOT /PASSWORD=${password}/   NOT password=(new_password) NOT /PASSWORD="$INPUT_PASSWORD"/ NOT /PASSWORD="$INPUT_APP_PASSWORD"/ NOT PASSWORD='password' NOT /PASSWORD="${ADMIN_PASSWORD:-password}"/ NOT /password=${env:SSL_KEYSTORE_PASSWORD}/ NOT password='" NOT password=' '  NOT Password=password  NOT password=%s NOT PASSWORD=$ NOT PASSWORD="***INVALID***" NOT PASSWORD="$ NOT password=<password> NOT TEST_GITHUB_PASSWORD= NOT password=" NOT password=secret</code> NOT password=options.password NOT user=%u&password=%p NOT PASSWORD=<your-password-here> NOT password=%v NOT PASSWORD=<admin-password> NOT password=qwerty )
```
