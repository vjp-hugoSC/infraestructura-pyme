# Copias de seguridad

## Base de datos

```bash
mysqldump -u root -p web_empresa > web_empresa.sql
```

## Archivos web

```bash
rsync -av /var/www/ /backups/web/
```

## Política de retención

- Diarias: 7 días
- Semanales: 4 semanas
- Mensuales: 12 meses