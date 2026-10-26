# Extractor de Facturas

Herramienta web para convertir facturas a CSV. Funciona en cualquier navegador (Windows, macOS, Linux).

## Qué hace

- Carga una carpeta (con todas sus subcarpetas), un ZIP o archivos sueltos.
- Lee facturas **CFDI 3.3 y 4.0** (XML) y **recibos de Meta Ads** (PDF).
- Genera un CSV con: Fecha, Folio, Proveedor, Concepto, Subtotal, Impuestos, Total, RFC Emisor y Archivo.
- Convierte los montos al formato mexicano (`1.427,07` → `1427.07`).
- Omite duplicados y los PDF que no son recibos de Meta.

## Privacidad

Todo se procesa en el navegador de quien la usa. Los archivos no se suben a ningún servidor y no se guarda nada.

## Librerías

Se cargan desde cdnjs con versión fija, no hay nada que instalar:

- [JSZip 3.10.1](https://stuk.github.io/jszip/): leer archivos ZIP.
- [pdf.js 3.11.174](https://mozilla.github.io/pdf.js/): leer el texto de los PDF.

## Actualizar

Edita `index.html` y haz commit. GitHub Pages publica el cambio en uno o dos minutos.
