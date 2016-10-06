# Email Server Checks

To make sure emails can reach its destinations, the following steps should be taken:

## Host configuration
- [ ] hostname is set to a FQDN
- [ ] hostname stays set after reboot (espacially relevant for virtual servers)

## DNS
- [ ] MX record points to the correct mail server
- [ ] Domain resolves to the correct IPv4
- [ ] Reverse DNS the IPv4 returns the Domain
- [ ] Domain resolves to the correct IPv6
- [ ] Reverse DNS the IPv6 returns the Domain

## SPF
The SPF record can be created using a tool like:

- [http://www.spf-record.de/generator](http://www.spf-record.de/generator)

- [ ] The SPF record was inserted into the Zone
- [ ] SPF contains IPv4 AND IPv6 AND any external server that may send our mail
- [ ] The correct configuration was verfified with a service like [https://www.mail-tester.com/](https://www.mail-tester.com/)
