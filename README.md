# Generador de Membretes/Firmas de Correo - Hospital Regional de Talca

Este es un proyecto sencillo y elegante para generar de forma automatizada las firmas de correo electrónico (membretes) institucionales de la **Unidad de Laboratorio** del **Hospital Regional de Talca**, diseñadas para ser utilizadas en **Gmail**.

La aplicación genera una firma en formato **HTML enriquecido** compatible con clientes de correo, asegurando que se visualice correctamente tanto en computadoras como en dispositivos móviles, manteniendo los colores y el logo institucional intactos.

---

## Estructura del Proyecto

* `index.html`: La aplicación web con el formulario de entrada, vista previa en tiempo real y lógica de copiado.
* `style.css`: Estilos visuales con una interfaz médica limpia, moderna y responsiva.
* `logo_cropped.png`: El logotipo institucional recortado y optimizado.
* `Pie-de-Firma-lab ARLETTE.png`: Plantilla de firma original utilizada como referencia.

---

## Cómo desplegar en GitHub Pages (Paso a Paso)

Para que el logotipo de tu firma se cargue correctamente en los correos que envíes a otras personas, la firma debe apuntar a una imagen alojada en internet. Alojar la aplicación en **GitHub Pages** soluciona esto de forma automática y gratuita.

Sigue estos sencillos pasos para publicarlo en tu cuenta de GitHub:

### Paso 1: Crear un Repositorio en GitHub
1. Inicia sesión en tu cuenta de [GitHub](https://github.com).
2. Haz clic en el botón **New** (Nuevo) para crear un nuevo repositorio.
3. Asigna un nombre al repositorio (por ejemplo: `membrete-hospital` o `firma-correo`).
4. Déjalo como **Public** (Público) —esto es necesario para que GitHub Pages sea gratuito y el logo se cargue públicamente—.
5. Haz clic en **Create repository** (Crear repositorio).

### Paso 2: Subir los Archivos
Puedes subir los archivos usando la interfaz web de GitHub o Git:

**Opción A: Subir por la Web (Más fácil si no usas Git en consola)**
1. En la página de tu repositorio vacío, haz clic en el enlace **"uploading an existing file"** (subir un archivo existente).
2. Arrastra y suelta los siguientes archivos de esta carpeta:
   * `index.html`
   * `style.css`
   * `logo_cropped.png`
3. Haz clic en **Commit changes** (Confirmar cambios).

**Opción B: Subir mediante Git en Consola**
Abre una terminal en esta carpeta y ejecuta:
```bash
git init
git add index.html style.css logo_cropped.png README.md
git commit -m "Initial commit: signature generator"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TU_REPOSITORIO.git
git push -u origin main
```
*(Reemplaza `TU_USUARIO` y `TU_REPOSITORIO` con tus datos de GitHub)*

### Paso 3: Activar GitHub Pages
1. Dentro de tu repositorio en GitHub, ve a la pestaña **Settings** (Configuración) arriba a la derecha.
2. En el menú lateral izquierdo, bajo la sección *Code and automation*, haz clic en **Pages**.
3. En la sección *Build and deployment*, busca **Source** y asegúrate de que esté en **Deploy from a branch**.
4. Debajo, en **Branch**, selecciona `main` (o `master`) y la carpeta `/ (root)`. Haz clic en **Save** (Guardar).
5. Espera aproximadamente 1-2 minutos. Al recargar la página, aparecerá un recuadro verde en la parte superior con un texto como:
   > *Your site is live at:* `https://tu_usuario.github.io/tu_repositorio/`

---

## Cómo usar el Generador

1. Abre el enlace proporcionado por GitHub Pages (`https://tu_usuario.github.io/tu_repositorio/`).
2. Completa los datos en el formulario:
   * **Nombre completo**: Se formateará en mayúsculas automáticamente.
   * **Cargo**: Es opcional. Si lo dejas en blanco, la firma se compactará y ocultará esta línea.
   * **Fono Directo** y **Anexo Minsal**: Son opcionales. Puedes ingresar uno de ellos, ambos, o dejarlos en blanco (en cuyo caso se omitirá por completo la línea telefónica).
3. La vista previa se actualizará en tiempo real.
4. Haz clic en **"Copiar Firma para Gmail"**.
5. Abre tu Gmail institucional y pega la firma (`Ctrl + V`) en la sección de configuración de firmas (Ajustes ⚙️ > Ver todos los ajustes > pestaña General > sección Firma).
6. ¡Guarda los cambios al final de la página de Gmail y listo!
