# alfonsoautomatiza.github.io

Alfonso Automatiza no está afiliado a Sage ni es distribuidor oficial. "Sage" y "Sage 50" son marcas registradas de The Sage Group plc.

Página índice (hub) de los manuales técnicos de las herramientas de Alfonso Automatiza:

- [S50Info](https://alfonsoautomatiza.github.io/S50info/)
- [Sage 50 BI](https://alfonsoautomatiza.github.io/Sage50bi/)
- [xls2sage50](https://alfonsoautomatiza.github.io/xls2sage50/)
- [RecWERTY](https://alfonsoautomatiza.github.io/recwerty/)
- [Backup Teamleader](https://alfonsoautomatiza.github.io/backup-crm-teamleader/)
- [Centralita IA Teamleader](https://alfonsoautomatiza.github.io/Centralita_Teamleader/)

Más información: [alfonsoautomatiza.com](https://alfonsoautomatiza.com/)

## Por qué existe este repo

Este repo publica la página de inicio de `alfonsoautomatiza.github.io` (GitHub Pages de usuario). Sirve para:

1. Dar una puerta de entrada única a los seis manuales (antes la raíz del dominio daba 404).
2. Servir un `robots.txt` y un `sitemap.xml` a nivel de todo el host — cada manual solo puede servir el suyo dentro de su propia subcarpeta, pero eso no lo consulta ningún rastreador real (el estándar solo revisa `robots.txt` en la raíz del host).
3. Permitir verificar **una sola** propiedad de prefijo de URL en Google Search Console y **un solo** sitio en Bing Webmaster Tools que cubra los seis manuales (y los que se añadan).

Detalle completo del análisis en la memoria del proyecto de Alfonso (`project_alfonsoautomatiza_manuales_seo`) y en `04_Marketing_Landing/MANUAL_INDEXACION_alfonsoautomatiza.md` §4 del proyecto `alfonsoautomatiza`.

## Pendiente conocido

El `sitemap.xml` publicado de **Sage50bi** todavía tiene URLs con el dominio antiguo `wertymsd.github.io` en vez de `alfonsoautomatiza.github.io` — pero el `site_url` en su `mkdocs.yml` fuente (`cerebro/000-PROYECTOS/010 - MANUALES/sage50bi/`) **ya está corregido**; solo falta redesplegar (`mkdocs gh-deploy --force` en esa carpeta) para que el sitio publicado se actualice.

Los repos fuente de **xls2sage50** y **Backup Teamleader** tienen su remoto `origin` apuntando todavía a la cuenta antigua `wertyMSD`, con un remoto adicional `publish` (SSH) apuntando a `alfonsoautomatiza`. `mkdocs gh-deploy` sin `--remote-name publish` empujaría a la cuenta equivocada — revisar antes de redesplegar esos dos.
