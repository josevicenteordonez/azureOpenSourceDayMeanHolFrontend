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