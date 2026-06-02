# Recuperación ante desastres

## Fallo del servidor web

1. Instalar Ubuntu.
2. Instalar Apache y PHP.
3. Restaurar archivos web.

## Fallo de base de datos

Restauración:

```bash
mysql -u root -p web_empresa < web_empresa.sql
```

## Objetivos

| Indicador | Valor |
|------------|--------|
| RTO | 4 horas |
| RPO | 24 horas |