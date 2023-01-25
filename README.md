# ansible-role-win-snmp

Role to install SNMP in Windows

## Table of content

- [Default Variables](#default-variables)
  - [win_snmp_auto_reboot](#win_snmp_auto_reboot)
  - [win_snmp_firewall_apply](#win_snmp_firewall_apply)
  - [win_snmp_firewall_open](#win_snmp_firewall_open)
  - [win_snmp_firewall_rules](#win_snmp_firewall_rules)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### win_snmp_auto_reboot

automatically reboot when required

#### Default value

```YAML
win_snmp_auto_reboot: true
```

### win_snmp_firewall_apply

#### Default value

```YAML
win_snmp_firewall_apply: true
```

### win_snmp_firewall_open

apply firewall rules

### win_snmp_firewall_rules

list of firewall rules to allow

#### Default value

```YAML
win_snmp_firewall_rules:
  - {name: SNMP UDP Port 161 In, direction: in, protocol: udp, localport: 161}
  - {name: SNMP UDP Port 161 Out, direction: out, protocol: udp, localport: 161}
  - {name: SNMPTRAP UDP Port 162 In, direction: in, protocol: udp, localport: 162}
  - {name: SNMPTRAP UDP Port 162 Out, direction: out, protocol: udp, localport: 162}
```



## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888
