# ProyectoNDA
Proyecto de gestión de autobuses para la provincia.
Software para la reserva y organización de plazas de autobús. Garantizando una organización eficiente y mezclando el control de reservas digital con la realidad física del autobús.
Este sistema permite a los usuarios:
-  Comprobar el número de asientos disponibles en su autobús en tiempo real.
-  La compra anticipada del billete o en el momento de entrar al autobús.

Para actualizar los asientos disponibles, la app genera un código de barras que deberá escanearse al entrar al autobús.
Para usuarios sin dispositivo móvil, se ofrecerá una tarjeta física con su propio código.

# Guía de instalación y despliegue: Requisitos

  ## 1-Como instalar.
  ### En iphone.
     Ir a la app Store buscar ProyectoNDA, desde ahi se puede descargar la aplicación.

   ### En android.
     Ir a la play store buscar ProyectoNDA, desde ahi se puede descargar la aplicación.

   ## 2-Requisitos.
     -Tener una red estable para su descarga
     -Camara con lector QR
     -2 Gb de ram para un rendimiento fluido
     -Espacio de entre 100-500mb de espacioç
     -GPS integrado

# Guia de estilos

## Colores:
Los colores usados son:
  - Morado oscuro: #6a4fa2 
  - Violeta: #8cd6fd
  - Azul: #e19afb
  - Azul claro: #b8ebfe
  - Blanco: #ffffff
    
## Tipografía:
  - Manjari
  - Conforta
    
## Componentes:
  - Lista seleccionables
  - Campos de texto
  - Campo fecha
  - Botones radio
  - Botones 
  - Enlaces
  - Switch
    
## Diseño responsive:
Diseño adaptado a dispositivos móviles desde  6,1 pulgadas a 6,7 pulgadas.

# Configuración de entorno
Este proyecto utiliza variables de entorno para manejar información sensible y configuraciones dependientes del entorno (como credenciales de base de datos y claves privadas).

DB_HOST=localhost
DB_PORT=5432
DB_NAME=usuariosEjemplo
DB_USER=adminEjemplo
DB_PASSWORD=contraseniaEjemplo

Por defecto se utiliza localhost y el puerto 5432.

Nuestros archivos .env seran añadidos a nuestro gitignore para que no puedan ser subidos a github, de esta forma los tendremos en forma local
y evitaremos publicarlos de forma erronea en nuestro github

# Comandos de ejecución 

### 1. Conectar vía SSH a tu servidor EC2
### 2. Actualizar paquetes y dependencias
### 3. Ejecutar el backend 
### 4. Conectar todas las API's necesarias

# Hosting. (Lo que pueda realizarse llegado a este punto a nivel técnico)

Este proyecto está desplegado en **Amazon Web Services (AWS)** utilizando una instancia **EC2** con **Apache** y **PHP 8.x** como lenguaje principal.  
La base de datos está gestionada en **AWS con PostgreSQL** para garantizar seguridad y escalabilidad.

### Configuración del servidor
- **Instancia EC2**: Amazon Linux 2 con Apache y PHP.
- **Base de datos**: PostgreSQL en RDS, accesible solo desde la instancia EC2.
- **Seguridad**:
  - Puertos abiertos: 80 (HTTP) y 443 (HTTPS).
  - Roles para acceso seguro a recursos.


