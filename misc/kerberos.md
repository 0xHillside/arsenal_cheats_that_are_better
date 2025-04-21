# Kerberos Time Skew

## Time Skew Using rdate
```
sudo rdate -n <IP_ADDRESS>
```

## Time Skew Using ntpdate
```
sudo ntpdate <IP_ADDRESS>
```

## Time Skew Using ntpdate
```
faketime "$(rdate -n 10.129.81.110 -p | awk '{print $2, $3, $4}' | date -f - "+%Y-%m-%d %H:%M:%S")" zsh
```
