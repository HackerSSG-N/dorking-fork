## When want to test target with shodan must run these queries

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
