# json-repo

Este repositorio contiene archivos JSON diseñados para [describir el propósito, uso o contexto de los JSON]. Cada archivo JSON está estructurado de manera que [explica brevemente la funcionalidad del JSON].

## Contenidos

- [`naming-convention.json`](#naming-conventionjson)

## Archivos

### `naming-convention.json`

Este archivo define listas y dependencias jerárquicas para la configuración de campañas, audiencias y formatos, que pueden ser utilizadas en diversas aplicaciones como automatización de marketing, gestión de datos y análisis.

#### **Estructura del Archivo**
El archivo incluye las siguientes claves principales:

- **`agenciaList`**: Lista de agencias disponibles.  
  Ejemplo: `["tca", "tcarx"]`

- **`clienteList`**: Lista de clientes asociados.  
  Ejemplo: `["promtur", "prom"]`

- **`divisionMarcaList`**: Listas de divisiones y marcas.  
  Ejemplo: `["promtur", "prom", "institutional", "branding"]`

- **`paisList`**: Países disponibles.  
  Ejemplo: `["arg", "blz", "bol", "bra", "can", ...]`

- **`tipoCompraList`**: Tipos de compra como "CPM", "CPC", entre otros.  
  Ejemplo: `["cpm", "cpc", "cpv", "cpa"]`

#### **Dependencias**
Algunos campos tienen dependencias jerárquicas, como las siguientes:

- **Fuente (`fuenteList`)**: Dependencias entre las fuentes y tipos de campaña.
  ```json
  "fuenteList": {
    "google": {
      "campaignTypes": {
        "search": ["paid-search"],
        "display": ["paid-display"]
      }
    }
  }

 ### Herramientas para ejecutar test
 Postman - Para probar el archivo como parte de una API (GET)
 Ir directamente al link: https://ac-tecea.github.io/json-repo/naming-convention.json
