# SSH y Firewall

## Configuración SSH

Editar:

```bash
sudo nano /etc/ssh/sshd_config
```

Configuración recomendada:

```text
PermitRootLogin no
PasswordAuthentication no
```

## Firewall UFW

```bash
ufw default deny incoming
ufw default allow outgoing

ufw allow from 192.168.1.0/24 to any port 22

ufw allow 80/tcp
ufw allow 443/tcp

ufw enable
```

## Comprobación

```bash
ufw status
```