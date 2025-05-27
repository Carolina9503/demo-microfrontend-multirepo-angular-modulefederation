# Activación de la federación de módulos para proyectos angular
El paquete @angular-architects/module-federation proporciona un generador personalizado. Si deseas aprender más de esta librería y arquitectura Angular visita el siguiente link: https://www.angulararchitects.io/en/aktuelles/the-microfrontend-revolution-module-federation-in-webpack-5/

Agregamos la librería en cada uno de los proyectos

# npm i -D @angular-architects/module-federation

Una vez instalada la librería agregaremos el uso de Module Federation a nuestros MF (microfrontends) y agregaremos unas configuraciones:

ng add @angular-architects/module-federation --project mf-shell --port 4200 --type host
ng add @angular-architects/module-federation --project mf-shopping --port 4201 --type remote
ng add @angular-architects/module-federation --project mf-payment --port 4202 --type remote
