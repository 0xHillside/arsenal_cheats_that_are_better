# FFUF 
#plateform/linux #target/remote #cat/enum



## FFUF subdomain checking
#plateform/linux #target/remote #cat/enum
```
ffuf -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-20000.txt -H "Host: FUZZ.<domain>.<ending>" -u https://<domain.here>
```


## FFUF Directory Fuzzing
#plateform/linux #target/remote #cat/enum
```
ffuf -w /usr/share/seclists/Discovery/Web-Content/raft-small-files.txt -u https://<domain.here>/FFUF
```

## FFUF Extensions
#plateform/linux #target/remote #cat/enum
```
ffuf -w /usr/share/seclists/Discovery/Web-Content/web-extensions.txt -u https://<domain.here>/<file>.FFUF
```