# simple-node-js-react-npm-app
#Jenkins

Este es el repo del articulo que esta en mi blog en Medium en español. 
[Build a Node.js and React app with npm](https://jenkins.io/doc/tutorials/build-a-node-js-and-react-app-with-npm/)
tambien pueden revisar la documentación oficial  [Jenkins User Documentation](https://jenkins.io/doc/).

Este repositorio contiene una apicación muy sencilla en Node.JS con React  la cual genera
una página web con el contenido "Welcome to React"  y es acompañada con ua prueba para revisar si 
la página "renderea" se dibuja satisfactoriamente.

El directorio  `jenkins` contiene el ejemplo ya final del flujo de trabajo -- es decir un pipeline  o `Jenkinsfile`
que bueno la idea es crearlo por nosotros mismo paso a paso durante el tutorial que pueden encontrar en mi blog. 

Enlace Medium AQUI

La sub carpeta  `scripts`  contiene los scripts en shell con los comandos que son ejecutados cuando Jenkins
procesa las etapas "Test" y "Deliver" , (las etapas o stages se pueden llamar como ustedes gusten) , pero pues 
es muy claro asi para que sirven cada una de estas en nuetsro pipeline. 

Alex
