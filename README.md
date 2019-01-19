# ANTI HOISTER
¡Ya no abran más hoisters en tu servidor!


# Instalación
Pasos para instalar el NPM:

- Debes tener **NPM**.
- Una vez en tu consola, debes poner `npm install anti-hoister`.
- Una vez instalado el NPM, vamos a ver como funciona.

# Funcionamiento
Para empezar a utilizar el NPM usted debera irse a el archivo principal de su bot. El cual puede ser **index.js**.

```js
// Código de arranque

const antihoist = require('anti-hoister');

antihoist(client, {
// Todos los mensajes se van a mostrar como un EMBED, lo cual abran más variables. Todos los embed tendran como titulo el nombre del hoister, es decir (Santiago) o el nombre del hoister!
msgWarn: "Es un hoister! Intentando remover su nombre...", // El mensaje que le lanzara al usuario si tiene un caracter de hoister. 
warnColor: "ORANGE", // Color del mensaje de advertencia.
msgSuccesfull: "¡Ya no tiene un nombre de hoister!", // El mensaje que editara el bot si la acción es valida.
succesfullColor: "GREEN", // Color del mensaje satisfactorio.
msgError: "Al parecer no tengo permisos para quitarle el nombre a ese hoister.", // El mensaje que editara el bot si la acción es inválida o ocurrio un error.
errorColor: "RED", // Color del mensaje erroneo.
bypass: ["Santiago#0001"], // Personas a las que no les afectara su nombre en hoist.
})
```

Si no quieres poner una opción, solo borra esa opción o variable. Ahora, si quieres que todo sea default solo pon:
```js
const antihoist = require('anti-hoister');
antihoist(client, {})
```
Asi de sencillo.

# Soporte
Si tienes problemas con el funcionamiento de este **NPM** puedes contactarme en Discord como **Santiago#0001**.
o Abrir un problema en nuestro [Github](https://github.com/magikste/anti-hoister)!