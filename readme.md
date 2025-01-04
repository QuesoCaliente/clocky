# Clocky

Este proyecto implementa un reloj digital de 24 horas diseñado especialmente para integrarse en OBS (Open Broadcaster Software), facilitando a streamers mostrar la hora en sus transmisiones en vivo. El reloj cuenta con soporte para diferentes zonas horarias de América Latina y puede personalizarse utilizando parámetros en la URL para mostrar la hora de una zona horaria específica y un emoji asociado.

## Características

- Muestra la hora en formato 24 horas.
- Compatible con múltiples zonas horarias de América Latina.
- Utiliza la configuración de zona horaria local de la computadora si no se especifica una zona horaria válida.
- Permite cambiar el emoji mostrado junto al reloj.

## Uso

Para utilizar el proyecto, puedes abrir el archivo HTML en tu navegador y personalizar la URL con los parámetros disponibles.

### Parámetros de URL

- **pais**: Define el país cuya zona horaria se usará. Si no se proporciona o no es válido, el reloj usará la zona horaria local de la computadora.
- **text**: Permite cambiar el emoji mostrado junto al reloj. Si no se proporciona, el valor predeterminado es `🐭` (ratón).

#### Ejemplos de uso

1. Hora en la Ciudad de México con emoji de taco:

   ```
   https://trinilup.github.io/clocky/?pais=Mexico&text=🌮

   ```

   Resultado: Muestra la hora de la Ciudad de México con un emoji de taco.

2. Hora en Chile con emoji predeterminado:

   ```
   https://trinilup.github.io/clocky/?pais=Chile
   ```

   Resultado: Muestra la hora de Santiago de Chile con el emoji predeterminado (🐭).

3. Hora local de la computadora (sin parámetros):

   ```
   https://trinilup.github.io/clocky/
   ```

   Resultado: Muestra la hora basada en la configuración de la zona horaria local de la computadora con el emoji predeterminado.

4. Hora local de la computadora con un emoji de queso:
   ```
   https://trinilup.github.io/clocky/?text=🧀
   ```
   Resultado: Muestra la hora basada en la configuración de la zona horaria local de la computadora con el emoji de queso.

## Lista de zonas horarias soportadas

- Argentina: `America/Argentina/Buenos_Aires`
- Bolivia: `America/La_Paz`
- Brasil: `America/Sao_Paulo`
- Chile: `America/Santiago`
- Colombia: `America/Bogota`
- CostaRica: `America/Costa_Rica`
- Cuba: `America/Havana`
- Ecuador: `America/Guayaquil`
- ElSalvador: `America/El_Salvador`
- Guatemala: `America/Guatemala`
- Honduras: `America/Tegucigalpa`
- Mexico: `America/Mexico_City`
- Nicaragua: `America/Managua`
- Panama: `America/Panama`
- Paraguay: `America/Asuncion`
- Peru: `America/Lima`
- RepublicaDominicana: `America/Santo_Domingo`
- Uruguay: `America/Montevideo`
- Venezuela: `America/Caracas`
- España: `Europe/Madrid`

## Requisitos

- Navegador moderno con soporte para `Intl.DateTimeFormat` y ES6.

## Licencia

Este proyecto es de uso libre y puede modificarse según tus necesidades.
