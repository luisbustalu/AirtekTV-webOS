# Airtek TV para webOS

Aplicación no oficial de LG webOS para ver los canales de Airtek TV. No está afiliada a Airtek.

La lista de canales sale de la API pública de Airtek. Las flechas mueven la guía, OK reproduce el canal seleccionado y Atrás vuelve a la guía. Un segundo Atrás cierra la aplicación.

## Instalación

El televisor tiene que tener el modo de desarrollador activado. La aplicación se instala desde un computador con [webOS Dev Manager](https://github.com/webosbrew/dev-manager-desktop/releases/latest).

1. En el televisor, instala **Developer Mode** desde LG Content Store e inicia sesión con la cuenta de desarrollador de LG. Activa el modo de desarrollador, enciende el servidor de claves y deja esa aplicación abierta. Ahí aparecen la dirección IP del televisor y la frase de acceso. La sesión caduca; renuévala desde la misma aplicación cuando ocurra.
2. En el computador, instala webOS Dev Manager para tu sistema desde su [última versión](https://github.com/webosbrew/dev-manager-desktop/releases/latest).
3. En webOS Dev Manager, agrega el televisor con esa dirección IP y la frase de acceso. El puerto de desarrollo es `9922`.
4. Descarga el `.ipk` de la [última versión de Airtek TV](https://github.com/luisbustalu/AirtekTV-webOS/releases/latest).
5. Selecciona el televisor en webOS Dev Manager, elige **Install** y abre el `.ipk` descargado.

El paquete se llama `ovh.anonimo.airtektvwebos_<version>_all.ipk`. Cuando termine la instalación, abre **Airtek TV** desde el lanzador del televisor.

## Versiones

Cada push a `main` o `master` empaqueta la aplicación y publica una versión en GitHub con la etiqueta de `appinfo.json`. El `.ipk` va adjunto a esa versión. Si se vuelve a subir la misma versión, el paquete de esa versión se reemplaza.

## Licencia

El código de la aplicación está bajo la [licencia MIT](LICENSE.md). hls.js se incluye bajo la licencia Apache 2.0. Esa licencia no cubre el nombre Airtek, los logos, la pantalla de inicio, los nombres de los canales ni las transmisiones: todo eso pertenece a sus respectivos dueños.
