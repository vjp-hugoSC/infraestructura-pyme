# Instalación del servidor web

## Actualización del sistema

```bash
sudo apt update
sudo apt upgrade -y
```

## Instalación Apache

```bash
sudo apt install apache2 -y
```

## Instalación PHP

```bash
sudo apt install php libapache2-mod-php php-mysql -y
```

## Verificación

```bash
systemctl status apache2
```

## Balanceador HAProxy

```bash
sudo apt install haproxy -y
```

HAProxy se utilizará para distribuir el tráfico web y mejorar la disponibilidad.