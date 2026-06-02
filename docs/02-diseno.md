# Diseño de la infraestructura

## Diagrama lógico

```text
Internet
    |
    v
+------------+
|  HAProxy   |
+------------+
      |
      v
+------------+
| Apache/PHP |
+------------+
      |
      v
+------------+
|   MySQL    |
+------------+
Componentes
Componente	Versión	Función
Ubuntu Server	22.04 LTS	Sistema operativo
Apache	2.4.60	Servidor web
PHP	8.2	Backend
MySQL	8.0	Base de datos
Netdata	Última estable	Monitorización
HAProxy	3.0	Balanceador
Certbot	2.9	SSL
Puertos
Puerto	Servicio
22	SSH
80	HTTP
443	HTTPS
3306	MySQL
19999	Netdata