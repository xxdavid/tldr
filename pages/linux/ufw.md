# ufw

> Uncomplicated Firewall.
> Frontend for iptables aiming to make configuration of a firewall easier.

- Enable ufw:

`ufw enable`

- Disable ufw:

`ufw disable`

- Show ufw rules:

`ufw status`

- Allow incoming traffic on port 5432 on this host:

`ufw allow {{5432}}`

- Allow traffic from 192.168.0.4 to port 22 using only tcp protocol:

`ufw allow from {{192.168.0.4}} to {{any}} port {{22}} proto {{tcp}}`

- Deny incoming traffic on port 80 on this:

`ufw deny {{80}}`

- Deny traffic to port 22 using only udp protocol:

`ufw deny from {{any}} to {{any}} port {{22}} proto {{udp}}`

- Delete the deny rule on port 80:

`ufw delete deny {{80}}`
