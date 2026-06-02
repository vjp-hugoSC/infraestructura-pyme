# Base de datos

## Instalación

```bash
sudo apt install mysql-server -y
```

## Creación de bases de datos

```sql
CREATE DATABASE web_empresa;
CREATE DATABASE gestion_interna;
```

## Creación de usuario

```sql
CREATE USER 'webuser'@'localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON web_empresa.* TO 'webuser'@'localhost';
FLUSH PRIVILEGES;
```