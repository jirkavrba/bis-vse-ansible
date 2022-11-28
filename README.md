## Ansible konfigurace pro semestrální práci z předmětu BIS

### Konfigurace ansible

- Nastavení hostname v `hosts.yml`, lze zkontrolovat přes `ansible -i ./hosts.yml all --list-hosts`
- Test připojení přes `ansible -i ./hosts.yml all -u xname00 -m ping`, kde `xname00` je jméno uživatele na serveru
- Změna hodnot v konfiguračním souboru `vars/default.yml`

Konfigurace může vypadat pro xname `vrbj04` a server `bis140.vse.cz` např. takto:

```yml
---
xname: "vrbj04"
email: "vrbj04@vse.cz"
server_host: "bis140.vse.cz"
server_conf: "bis140-vse-cz.conf"
```