# \<credit-connection\>

Connection for the credit ui component and the backend API.

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

## Properties

### Custom properties

|Custom property  | Description   |
|---------------- |:-------------:|
|api    | titulo que se pinta sobre el header del formulario|
|params    | titulo o leyenda que se pinta sobre el footer|
|method    | url de la api que se va consumir a traves del componente|
|body   | body de la peticion que se va a realizar con base en los formulario|
|config   | propiedad usada cuando no se tiene un api realiza el calculo basico de un prestamo personal|
|request   | objeto json para realizar el consumo de la API|


## Methods

### Custom events

|Custom property  | Description   | Parametros |
|---------------- |:-------------:|:----------:|
|generateRequest  | metodo que genera la peticion a la API si es que se encuentra seteada la propiedad url| ninguno|
|_handleResponse  | metodo invocado cuando se obtiene la respuesta de la API| event|
|_handleError  | metodo que se invoca cuando hay un error al realizar la petición| event|
|_creditAvailabilityCheck | metodo invocado cuando no se tiene o proporciona una API| ninguno|
|_getCreditWithInterest  | metodo que calcula el precio total| ninguno|
|_getMonthlyPayWithInterest | metodo que calcula el precio del pago mensual| response|
|_getIncomePayLimit  | metodo que calcula el monto minimo requerido para solicitar el prestamo | ninguno|
