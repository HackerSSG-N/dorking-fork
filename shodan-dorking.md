## When want to test target with shodan must run these queries
```bash
ssl.cert.subject.CN:"*.target.com"
```
```bash
Ssl.cert.subject.CN:"redacted.com" http.title:"IIS"
```
```bash
asn= AS12345 http.title:"redacted"
```
```bash
ip= 127.0.0.1 http.title:"redacted"
```
```bash
Ssl.cert.subject.CN:"redacted.com" http.title:"index of/"
```
```bash
Ssl.cert.subject.CN:"redacted.com" http.title:"gitlab"
```
```bash
Ssl.cert.subject.CN:"redacted.com" "230 login successful" port:"21"
```
```bash
Ssl.cert.subject.CN:"*.redacted.com"+200 http.title:"Admin"
```

## Open instances of Jenkins
```bash
Ssl.cert.subject.CN:"redacted.com" x-jenkins 200
```

## Open instances of  Sonarqube
```bash
Ssl.cert.subject.CN:"redacted.com" http.favicon.hash:”1485257654"
```

## Admin panels
```bash
ssl.cert.subject.cn:"company.com" http.title:"admin"
```
```bash
ssl:"company.com" http.title:"admin"
```
```bash
ssl.cert.subject.cn:"company.com" admin
```
```bash
ssl:"company.com" admin
```
## Telnet to root access to terminal
```bash
Ssl.cert.subject.CN:"redacted.com" "root@" port:23 -login -password -name -Session
```

## Mongo DB
```bash
Ssl.cert.subject.CN:"redacted.com" "Set-Cookie: mongo-express=""200 OK"
```
## Default Directory Listing
```bash
Ssl.cert.subject.CN:"redacted.com" http.html:"index of /"
```

## Backup Files
```bash
Ssl.cert.subject.CN:"redacted.com" http.html:"index of /" http.html:"backup"
```

## Compressed Achives
```bash
http.html:"index of /" http.html:"tar.gz"
```

## Database files
```bash
http.html:"index of /" http.html:"database"
http.html:"index of /" http.html:".sql"
http.html:"index of /" http.html:".db"
http.html:"index of /" http.html:"db_backup"
http.html:"index of /" http.html:"mysql.dump"
http.html:"index of /" http.html:".mdb"
```

## Configuration files
```bash
http.html:"index of /" http.html:".xml"
http.html:"index of /" http.html:"config.xml"

#tomcat: db connection strings
http.html:"index of /" http.html:"server.xml"
```

## Wordpress Configuration Files
```bash
http.html:"index of /" http.html:"wp-config.php.txt"
http.html:"index of /" http.html:"wp-config.txt"
http.html:"index of /" http.html:"wp-config.php.bak"
http.html:"index of /" http.html:"wp-config.php.old"
http.html:"index of /" http.html:"wp-config.php.backup"
http.html:"index of /" http.html:"wp-config.php.zip"
http.html:"index of /" http.html:"wp-config.php.tar.gz"
```

## Passwords
```bash
http.html:"index of /" http.html:"pwd"
http.html:"index of /" http.html:"pass.txt"
http.html:"index of /" http.html:"password"
http.html:"index of /" http.html:"password.txt"
http.html:"index of /" http.html:"passwords.txt"
http.html:"index of /" http.html:"passwords.zip"
```

## Windows Server Config Files
```bash
http.html:"index of /" http.html:"web.config"
```

## Exposed Logs
```bash
http.html:"index of /" http.html:".log"
http.html:"index of /" http.html:"access.log"
http.html:"index of /" http.html:"error.log"
http.html:"index of /" http.html:"php_error.log"
http.html:"index of /" http.html:"debug.log"
```

## Configuration and Version Control Files
```bash
http.html:"index of /" http.html:".env"
http.html:"index of /" http.html:".svn"
```

## Git Repositories
```bash
http.html:"index of /" http.html:".git"
http.html:"index of /" http.html:"gitconfig"
```

## Exposed Docker Registry API Without Authentication
```bash
"Docker Registry HTTP API" -"UNAUTHORIZED"
```

## DRUPAL TAKEOVER
```bash
http.html:"Set up database" http.html:"Drupal"
http.title:"Select an installation profile"
```

## SSO Login (Single Sign-On)
```bash
http.html:"SSO Login"
http.html:"Login with SSO"
http.html:"Single Sign-On"
```

## spring boot (if found something so fuzz with that using ffuf will get a P1  bounty)
```bash
http.favicon.hash:"116323821"
```
```bash
/actuator/env
/actuator/auditevents
/actuator/beans
/actuator/caches
/actuator/configprops
/actuator/flyway
/actuator/health
/actuator/heapdump
/actuator/httptrace
/actuator/info
/actuator/integrationgraph
/actuator/liquibase
/actuator/configprops
/actuator/shutdown
```


