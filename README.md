# FabCar

## ¿Qué es FabCar?
FabCar es una aplicación basada en web destinada a proporcionar una interfaz gráfica de usuario para la aplicación Fabcar presentada en Hyperledger Fabric [tutorial "Escribiendo su primera aplicación"] (https://hyperledger-fabric.readthedocs.io/en/release-1.2 /write_first_app.html).

## Cómo configurar FabCar
1. Siga el tutorial de Hyperledger Fabric para instalar Fabric y sus dependencias relacionadas.
2. Una vez hecho esto, siga el tutorial que se encuentra en [esta página] (https://hyperledger-fabric.readthedocs.io/en/release-1.2/write_first_app.html) hasta justo antes de la parte "Consultar el libro mayor".
3. Coloque el archivo "fabcar-backend.js" en el mismo directorio que los archivos Hyperledger "registerUser.js" y "enrolAdmin.js". Inicie el servidor Express con el siguiente comando.
     `` sh
    $ nodo fabcar-backend.js
    `` `
4. Una vez que el servidor express esté activo, compile y ejecute el front-end React que se encuentra en la carpeta "fabcar-front".
5. FabCar debería estar disponible en localhost: 3000

## Cómo usar FabCar
La interfaz FabCar se divide en tres pantallas separadas; la pantalla de información superior izquierda, la pantalla de navegación superior derecha y el visor de bloque inferior.

Cuando la aplicación se inicia por primera vez, el último bloque se recuperará del libro mayor y se agregará a la lista de bloqueo.
También habrá un pequeño indicador de estado en la esquina inferior derecha para indicar si la aplicación está conectada al servidor de fondo.

FabCar tiene 4 funciones principales:

- Consulta un solo auto
- Consulta todos los autos
- Transferir un auto
- Crea un auto

Estas funciones reflejan la aplicación fabcar original basada en la línea de comandos que se encuentra en la documentación de Hyperledger.
