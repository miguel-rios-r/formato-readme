REGLAS PARA EL CÓDIGO Y EL DESARROLLO
-

## Variables

### Reglas:

- Que totalmente prohibido el uso de *var* para la inicialización  de variables. 
- Para iniciar una variable es obligatorio usar *let*.
- Para datos que no vayan a mutar, es obligatorio usar *const*.
- La notación a utilizar para las variables es Camel Case.
- La notación a utilizar para las constantes es Uppercase.
- Los nombres de variables deben ser totalmente descriptivos y sin abreviaciones de ningún tipo.
- Todas las variables deben ser inicializadas con el valor de null a menos que se requiera. 

### Razón:

- Esta regla trata de evitar problemas por el efecto “Hoisting” de Javascript, limitando el uso de las variables a su scope, evitar confusiones por nombres de variables y evitar mutación de datos no variables. 

### Ejemplos:

- NO: var mivariable
- NO: var mi-variable
- SI: let miVariable = null
- NO: const miConstante
- SI: const MICONSTANTE


## Funciones

### Reglas:

- Es obligatorio el uso de Arrow Functions, utilizando la notación mínima del caso de uso.
- Los nombres de las funciones deben estar descritas en Pascal case. 

### Razón:

- Estandarizar el código y lograr legibilidad de código.

### Ejemplos:

- NO: function miFuncion() {}
- SI: const MiFuncion = () => {}
- NO: const MIFUNCION = () => {}


## Validaciones

### Reglas:

- Queda totalmente prohibidas las validaciones genéricas de doble igual == .
- Es obligatorio el uso de validaciones específicas de dato y tipo (de triple igual).

### Razón:

- Las validaciones específicas evitan falsos “true” como respuesta de comparaciones.

### Ejemplos:

- NO: varA == varB
- SI: varA === varB

## Bucles

## Reglas:

- Está prohibido el uso de cliclos (FOR, WHILE y DO WHILE).
- Es obligatorio el uso de MAP, REDUCE, FILTER y demás métodos de Arrays.
- Se admite el uso de iteradores (FOR, WHILE, DO WHILE) solo si se justifica con razones relevantes.


## Branch

### Reglas: 

- Es obligatorio el uso de ramificación por funcionalidad.
- El nombre del branch debe ser descriptivo a lo desarrollado, sin ningún tipo de abreviación, seguido del identificador “feature”.
-  La notación a utilizar es Lower case, con las palabras separadas con “-”.

### Ejemplos:
- NO: estoEsUnBranch
- SI: nuevo-branch-feature


## Recomendaciones:
- Estas reglas deben ser cumplidas para que los “Pull Request” a la rama Master sean aceptados, internamente, puede trabajar de la manera que mejor le convenga. Se recomienda implementar estas reglas en los ramas locales, pero no es obligatorio.



SOBRE EL PROYECTO
-

Este proyecto se inició con [Crear aplicación React] (https://github.com/facebook/create-react-app).

## Scripts disponibles

En el directorio del proyecto, puede ejecutar:

### `yarn start`

Ejecuta la aplicación en modo de desarrollo.<br />
Abrir [http://localhost:3000](http://localhost:3000) para verlo en el navegador.

La página se volverá a cargar si realiza modificaciones.<br />
También verá cualquier error en la consola.

### `yarn test`

Inicia el corredor de prueba en el modo de reloj interactivo. <br />
Consulte la sección sobre [pruebas en ejecución] (https://facebook.github.io/create-react-app/docs/running-tests) para obtener más información.

### `yarn build`

Crea la aplicación para producción en la carpeta `build`. <br />
Empaqueta correctamente React en modo de producción y optimiza la compilación para obtener el mejor rendimiento.

La compilación se minimiza y los nombres de archivo incluyen los hashes. <br />
¡Tu aplicación está lista para implementarse!

Consulte la sección sobre [deploy] (https://facebook.github.io/create-react-app/docs/deployment) para obtener más información.

### `yarn eject`

**Nota: esta es una operación unidireccional. Una vez que "expulsa", ¡no puede regresar!**

Si no está satisfecho con la herramienta de compilación y las opciones de configuración, puede "expulsar" en cualquier momento. Este comando eliminará la dependencia de compilación única de su proyecto.

En su lugar, copiará todos los archivos de configuración y las dependencias transitivas (paquete web, Babel, ESLint, etc.) directamente en su proyecto para que tenga control total sobre ellos. Todos los comandos excepto `eject` seguirán funcionando, pero apuntarán a los scripts copiados para que pueda modificarlos. En este punto, estás solo.

No tiene que usar nunca `expulsar`. El conjunto de funciones seleccionadas es adecuado para implementaciones pequeñas y medianas, y no debe sentirse obligado a usar esta función. Sin embargo, entendemos que esta herramienta no sería útil si no pudiera personalizarla cuando esté listo para ello.

## Aprende más

Puede obtener más información en la [Crear documentación de la aplicación React] (https://facebook.github.io/create-react-app/docs/getting-started).

Para aprender React, consulte la [Documentación de React] (https://reactjs.org/).

### División de código

Esta sección se ha movido aquí: https://facebook.github.io/create-react-app/docs/code-splitting

### Analizando el tamaño del paquete

Esta sección se ha movido aquí: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Hacer una aplicación web progresiva

Esta sección se ha movido aquí: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Configuración avanzada

Esta sección se ha movido aquí: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Implementación

Esta sección se ha movido aquí: https://facebook.github.io/create-react-app/docs/deployment

### `yarn build` falla al minificar

Esta sección se ha movido aquí: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify

