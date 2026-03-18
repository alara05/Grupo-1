# BASE DE DATOS – COOPERATIVAS DE TRANSPORTE

## Herramienta utilizada
Para el desarrollo de la solución se puede utilizar:

- **Draw.io** o **diagrams.net** para el modelo entidad-relación
- **Visual Studio Code** para redactar la documentación y el esquema lógico
- **MySQL Workbench** o cualquier editor SQL para representar las tablas

## Descripción del caso
Se desea crear una base de datos para controlar los viajes de las cooperativas de transporte hacia las diferentes ciudades del país.

De las cooperativas de transporte se conoce:
- código
- nombre
- dirección
- teléfono

Una cooperativa tiene muchos socios, pero un socio puede pertenecer solo a una cooperativa.

De cada socio se conoce:
- cédula
- nombre
- apellido
- dirección
- teléfono
- fecha de nacimiento

Un socio tiene muchas unidades (buses), pero una unidad pertenece solo a un socio.

De cada unidad (bus) se conoce:
- número de disco (id)
- marca
- año
- placa
- capacidad de pasajeros

Una provincia tiene muchos cantones, pero un cantón pertenece solo a una provincia.

De cada provincia se conoce:
- código
- nombre
- ubicación

De cada cantón se conoce:
- código
- nombre
- referencia geográfica

Muchos buses viajan a muchos cantones. De cada viaje se conoce:
- número de viaje
- fecha hora de salida
- fecha hora de llegada
- costo del asiento
- cantidad de pasajeros que viajan

A los buses se les realizan controles de calidad anuales. Un bus pasa varios controles y un control se aplica a un solo bus.

Del control se conoce:
- código
- fecha del control
- tipo de control
- id del funcionario responsable
- resultado del control (aprobado o reprobado)

Un control puede tener muchos incumplimientos.

De cada incumplimiento se conoce:
- id
- descripción
- nivel de gravedad de la novedad

## Objetivo
Desarrollar la solución de base de datos hasta el **esquema lógico**, incluyendo:
1. Identificación de entidades
2. Cardinalidades
3. Conversión a tablas
4. Revisión de integridad