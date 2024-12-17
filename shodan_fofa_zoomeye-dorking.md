## When want to test target with shodan must run these queries

```bash
Ssl.cert.subject.CN:”redacted.com” http.title:”IIS”
```
```bash
asn= AS12345 http.title:”redacted”
```
```bash
ip= 127.0.0.1 http.title:”redacted”
```
```bash
Ssl.cert.subject.CN:”redacted.com” http.title:”index of/”
```
```bash
Ssl.cert.subject.CN:”redacted.com” http.title:”gitlab”
```
```bash
Ssl.cert.subject.CN:”redacted.com” “230 login successful” port:”21"
```
```bash
Ssl.cert.subject.CN:”*.redacted.com”+200 http.title:”Admin”
```

## Open instances of Jenkins
```bash
x-jenkins 200
