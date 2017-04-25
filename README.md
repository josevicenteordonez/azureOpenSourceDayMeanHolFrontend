# azureOpenSourceDayMeanHolFrontend
Código angularjs para la solución del frontend corriendo en Azure.

# Parte II: Construir Solución Frontend con Angular-Cli

## Instalación y Creación de proyecto Angular-Cli ##
1.  Primero instalamos el modulo npm de angular cli de manera global con el siguiente comando

`npm install -g @angular/cli`

2.  Una vez instalado podemos utilizar el comando `ng` en nuestra terminal para crear un nuevo proyecto angular

`ng new appContactos`

3.  Ingresamos al nuevo directorio creado appContactos y ejecutamos el siguiente comando

`ng serve`

4. Luego podemos navegar al la página [http://localhost:4200/](http://localhost:4200/) y veremos nuestra aplicación corriendo

## Testing de Nuestro Código Angular ##

1.  Ahora que tenemos nuestro código podemos ejecutar pruebas unitarias usando el siguiente comando
`ng test`

Para una sola corrida podemos usar:

`ng test --single-run`

2.  También podemos hacer pruebas end to end utilizando los siguientes comandos:
`ng serve`
`ng e2e`

Para poder correr las pruebas end to end, se usa la herramienta protractor y para ello la app debe estar corriendo en el servidor.

3.  Y también podemos ejecutar typescript lint para verificar buenas prácticas de escritura de código typescript con el siguiente comando:
`ng lint`

## Construcción de Nuestro Código Angular ##

1.  Para poder generar codigo para distribuir lo podemos hacer de dos maneras:
    1.  Para entornos de prueba con posibilidad de debuggear, usamos el siguiente comando:
        `ng build`
        Esto generar el codigo resultante en una nueva carpeta llamada `dist`
    2.  Para entornos productivos, angular-cli puede generar un output completamente, minificado, ofuscado utilizando webpack. Para ello debemos usar el comando:
        `ng build --prod`

## Modificación de codigo para conectarse a nuestra API ##

1.  Modificar acceso CORS de nuestra API en Azure

![alt text][modificacionCors]

[modificacionCors]: https://raw.githubusercontent.com/feranto/azureOpenSourceDayMeanHol/master/imagenes/CORS.PNG "Modificación CORS"


2.  Crear un nuevo "servicio" de angular, para ello ejecutamos los siguientes comandos:
`ng generate service contactsService`

3.  Modificar la vista para poder listar todos los contactos
4.  Conectar la vista con el servicio
5.  Modificar la vista para poder listar un contacto por ID
6.  Conectar la vista con el servicio para obtener un contacto por ID

## Deployar en Azure ## 

1.  Crear AppService
![alt text][]

[]: https://raw.githubusercontent.com/feranto/azureOpenSourceDayMeanHol/master/imagenes/CORS.PNG ""
2.  Crear AppService Plan
![alt text][]

[]: https://raw.githubusercontent.com/feranto/azureOpenSourceDayMeanHol/master/imagenes/CORS.PNG ""
3.  Deployar Codigo
![alt text][]

[]: https://raw.githubusercontent.com/feranto/azureOpenSourceDayMeanHol/master/imagenes/CORS.PNG ""
4.  Probar aplicación
![alt text][]

[]: https://raw.githubusercontent.com/feranto/azureOpenSourceDayMeanHol/master/imagenes/CORS.PNG ""
