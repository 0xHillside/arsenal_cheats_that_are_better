# KeyTab file for evil-winrm

## the file
```
cat << 'EOF' > krb5.conf

[libdefaults]
    default_realm = <DOMAIN.NAME>

# The following krb5.conf variables are only for MIT Kerberos.
    kdc_timesync = 1
    ccache_type = 4
    forwardable = true
    proxiable = true
    rdns = false

# The following libdefaults parameters are only for Heimdal Kerberos.
    fcc-mit-ticketflags = true

[realms]
    VINTAGE.HTB = {
        kdc = <FQDN.DOMAIN.NAME>
        admin_server = <FQDN.DOMAIN.NAME>
    }

[domain_realm]
    .<domain.name> = <DOMAIN.NAME>
    <domain.name> = <DOMAIN.NAME>
EOF
```

