# Proyecto de Comparación de Comunidades Autónomas y Ciudades de España

Este proyecto permite realizar una comparación entre comunidades autónomas y ciudades de España. La comparación se puede realizar de dos maneras: utilizando una llamada a una API externa o mediante un diccionario local de ciudades y sus respectivos valores.

## Características

- **Comparación de comunidades autónomas y ciudades**: Se asigna un valor a la variable `ciudad` según la comunidad autónoma seleccionada.
- **Flexibilidad en la integración**: Puedes elegir entre realizar la comparación utilizando una API externa o un diccionario local de ciudades.

## Vista previa del proyecto

Puedes visualizar cómo queda el proyecto visualmente en el siguiente enlace de Behance:  
[Calculadora de Alquiler Vacacional en Behance](https://www.behance.net/gallery/223405579/Calculadora-de-Alquiler-Vacacional).

## Métodos de Comparación

### 1. Llamada a la API

La comparación se puede realizar mediante una llamada a la API de PlaceKit o una API similar, obteniendo datos de comunidades autónomas y ciudades en tiempo real. Si optas por este método, asegúrate de obtener una clave API y reemplazar el marcador de posición en el código.

#### Obtener la clave API

- Ve a [PlaceKit API](https://app.placekit.io/) para obtener tu clave API.

#### Configuración en el código

Reemplaza `'aqui-va-mi-clave-API-key='` por tu clave API en el siguiente fragmento de código:

```javascript
const pka = placekitAutocomplete('aqui-va-mi-clave-API-key=TU_CLAVE_API', {
  target: '#address',
  language: 'es',
  countries: ['es'],
});
