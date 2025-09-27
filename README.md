![Logo PDFina](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/icon.png)

# Guía de inicio en PDFina

A continuación encontrarás una guía rápida con imágenes para comprender el uso de **PDFina**, nuestra aplicación de escritorio para trabajar con archivos PDF.

---

### `Nota importante sobre antivirus`

Si utilizas **Windows Defender**, la instalación no presentará inconvenientes. Puede aparecer en pantalla un aviso de análisis durante la instalación, lo cual es un comportamiento **normal**.

En caso de que tengas **Avast** u otro antivirus que muestre advertencias, recomendamos **desactivarlo temporalmente durante la instalación o actualización** y posteriormente añadir las siguientes rutas como **excepciones**:
```
C:\Users\TU_USUARIO\AppData\Local\Programs\pdfina\resources\app.asar.unpacked\resources\app\microservicios\pdf-a-word\dist\mservice-paw.exe
```
```
C:\Users\TU_USUARIO\AppData\Local\Programs\pdfina\resources\app.asar.unpacked\resources\app\microservicios\word-a-pdf\dist\mservice-wap.exe
```
```
C:\Users\TU_USUARIO\AppData\Local\Programs\pdfina\resources\app.asar.unpacked\resources\app\vendor\laravel\framework\src\Illuminate\Foundation\resources\server.php
```

#### ¿Cómo saber tu nombre de usuario en Windows?
El texto `TU_USUARIO` corresponde a tu usuario de Windows. Para identificarlo:
1. Abre el **Explorador de archivos**.  
2. Ve a `C:\Users\`.  
3. Allí verás una carpeta con el nombre de tu usuario actual (ejemplo: `Laura`, `Admin`, etc.).  
Ese es el valor que debes reemplazar en las rutas.

#### ¿Por qué aparece esta advertencia?
Los archivos señalados corresponden a los **microservicios internos** que permiten la conversión de:
- **Word → PDF**  
- **PDF → Word**  

Estos ejecutables aún **no cuentan con firma digital**, lo cual es habitual en proyectos nuevos y puede generar falsos positivos en algunos antivirus. Este detalle será subsanado en futuras versiones.

#### Sobre `server.php`
En algunos casos, el antivirus puede marcar el archivo:
```
C:\Users\TU_USUARIO\AppData\Local\Programs\pdfina\resources\app.asar.unpacked\resources\app\vendor\laravel\framework\src\Illuminate\Foundation\resources\server.php
```
como sospechoso.  
Esto es un **falso positivo**:  
- Se trata de un archivo legítimo del **framework Laravel**, utilizado por PDFina.  
- Los antivirus lo interpretan erróneamente como un script de servidor desconocido debido a su nombre (`server.php`) y a que se ejecuta en segundo plano para manejar procesos internos.  
- No representa ningún riesgo para tu equipo.  

>En resumen: estas advertencias son normales en proyectos nuevos sin firma digital, y no afectan la seguridad ni el funcionamiento de tu sistema. No olvides que el texto `TU_USUARIO` corresponde a tu usuario de Windows.

![Foto1](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto1.png)

Si es tu primera vez utilizando **PDFina**, debes registrarte.  
Quizás te preguntes: *“Si PDFina no requiere conexión a Internet, ¿por qué debo registrarme?”*  
La respuesta es sencilla: los datos se almacenan **localmente en tu computadora** para guardar tus preferencias, como el modo claro, oscuro y otras configuraciones personales.

---

![Foto2](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto2.png)

Dado que no se envía información a Internet, puedes utilizar incluso un correo ficticio si lo deseas.  
Respecto a la contraseña, recuerda que debe ser **alfanumérica** para mayor seguridad.

---

![Foto3](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto3.png)

Una vez que te registres, ingresarás directamente al **panel principal**, donde encontrarás un **menú lateral izquierdo** que te permitirá seleccionar el módulo que necesites.

---

![Foto4](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto4.png)

En la parte inferior de este menú tendrás opciones adicionales:  
- Reportar problemas  
- Enviar sugerencias sobre nuevas funcionalidades  
- Vaciar la papelera (lo veremos más adelante)  
- Consultar la documentación, donde podrás volver a repasar estos pasos  

---

![Foto5](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto5.png)
![Foto6](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto6.png)
![Foto7](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto7.png)
![Foto8](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto8.png)

Dentro de tu configuración personal podrás:  
- Cambiar la contraseña  
- Eliminar tu cuenta  
- Modificar la apariencia (modo claro/oscuro)  

---

![Foto9](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto9.png)

Para salir de la aplicación puedes:  
- Ir al menú superior → **Archivo → Salir de PDFina**  
- O bien, hacer clic en el botón **cerrar ventana** (esquina superior derecha).  

---

![Foto10](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto10.png)

Para utilizar el módulo de **compresión de PDF** es necesario tener instalado [**Ghostscript**](https://ghostscript.com/releases/gsdnld.html) en tu sistema.  
- Descarga la versión para **Windows 64 bits** desde la página oficial.  
- Una vez instalado, cierra y vuelve a abrir **PDFina** para activar esta función.  

---

![Foto11](https://raw.githubusercontent.com/matiaslawwliet/PDFina-releases/refs/heads/main/img/foto11.png)

Actualmente, **PDFina** se encuentra en **fase Beta**.  
Algunas acciones, como la **eliminación de archivos temporales**, deben hacerse manualmente.  
Estos archivos son copias creadas durante procesos de conversión o compresión.  
No olvides **vaciar la papelera de PDFina** periódicamente para mantener tu sistema limpio.  

---
Gracias por confiar en **PDFina** ❤️