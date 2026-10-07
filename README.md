# Cómo publicar la Política de Privacidad de ElCambio VE

Esta carpeta (`privacidad/`) contiene la política de privacidad de la app **ElCambio VE** lista para publicar en internet.
Esta guía está escrita para alguien que **no programa**: solo hay que copiar, pegar y hacer clic. No necesitas instalar nada.

---

## 0. Qué hay en esta carpeta

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | La política como **página web**. Es el archivo que se publica y el que verá Google Play. Está completo: no necesita internet, ni archivos extra, ni programas. |
| `PRIVACY.md` | El mismo texto en formato Markdown, para que quede guardado dentro del repositorio del proyecto. |
| `README.md` | Esta guía (la que estás leyendo). |

> Puedes abrir `index.html` haciendo doble clic: se verá igual que en internet.

---

## 1. ANTES DE PUBLICAR: reemplaza los dos marcadores

La página tiene dos textos entre corchetes que **debes cambiar por tus datos reales**. Si no los cambias, tu política se publicará con corchetes y Google Play puede rechazarla.

| Marcador | Qué poner |
| --- | --- |
| `[NOMBRE DEL RESPONSABLE]` | Tu nombre completo, o el nombre de tu negocio/marca. Si prefieres no publicar tu nombre, puedes escribir algo como «Desarrollador de ElCambio VE». |
| `[CORREO DE CONTACTO]` | Un correo electrónico real que revises, por ejemplo `elcambiove@gmail.com`. |

**Dónde están:** aparecen varias veces en las secciones 1, 8, 9, 11, 12 y 13, y también en el recuadro de datos de la cabecera, tanto en `index.html` como en `PRIVACY.md`. Al final de la página web hay un aviso azul y al final del Markdown un comentario: **bórralos cuando termines** (el aviso azul se ve en la web publicada).

**Cómo cambiarlos, paso a paso (sin programas):**

1. Abre `index.html` con el Bloc de notas (clic derecho sobre el archivo → *Abrir con* → *Bloc de notas*).
2. En el Bloc de notas pulsa `Ctrl + H` (Buscar y reemplazar).
3. En «Buscar» escribe `[NOMBRE DEL RESPONSABLE]` y en «Reemplazar por» tu nombre. Pulsa *Reemplazar todo*.
4. Repite con `[CORREO DE CONTACTO]` y tu correo. Pulsa *Reemplazar todo*.
5. Borra el párrafo del final que empieza con **«Nota para quien publica esta página»** (borra desde `<p class="note-editable">` hasta `</p>` justo antes de `<footer>`).
6. Guarda con `Ctrl + G` y cierra.
7. Haz lo mismo en `PRIVACY.md` (y borra el comentario final entre `<!--` y `-->`).

> **Truco:** los corchetes `[ ]` son solo para que veas fácilmente qué falta. Al reemplazar, escribe el dato **sin** corchetes.

---

## 2. Publicar en GitHub Pages (gratis)

GitHub es una web donde se guardan archivos, y **GitHub Pages** es el servicio gratuito que los muestra como página web.

> ⚠️ **Importante:** en las cuentas gratuitas, GitHub Pages solo funciona con repositorios **públicos**. Eso significa que **todo lo que subas a ese repositorio será visible para cualquiera**. Si subes la carpeta completa del proyecto de la app, tu código quedará público.
>
> ✅ **Recomendado:** crea un repositorio nuevo y **solo para la política** (por ejemplo `elcambio-privacidad`) y sube ahí únicamente el archivo `index.html`. Así tu código queda privado y tu política queda publicada.

### Paso 2.1. Crear la cuenta de GitHub (si no tienes)

1. Entra a `https://github.com` y pulsa **Sign up**.
2. Elige un nombre de usuario (por ejemplo `elcambiove`). **Recuérdalo**: formará parte de la dirección de tu política.
3. Confirma tu correo.

### Paso 2.2. Crear el repositorio

1. Ya con la sesión iniciada, pulsa el botón **+** (arriba a la derecha) → **New repository**.
2. En **Repository name** escribe: `elcambio-privacidad`
3. En **Description** (opcional): `Política de privacidad de ElCambio VE`.
4. Marca la opción **Public**.
5. Pulsa **Create repository**.

### Paso 2.3. Subir el archivo `index.html`

1. En la página del repositorio recién creado, pulsa el enlace **uploading an existing file** (o el botón **Add file → Upload files**).
2. **Arrastra** el archivo `index.html` desde la carpeta `privacidad` de tu computadora hasta la ventana del navegador.
   - También puedes copiar **todo el contenido de la carpeta `privacidad`** (los 3 archivos) si quieres guardar la versión Markdown y esta guía.
   - Si quieres que la dirección sea más corta, sube `index.html` **en la raíz** del repositorio (no dentro de una subcarpeta). Es lo más simple y lo recomendado.
3. Abajo, en **Commit changes**, escribe un texto como `Publicar política de privacidad` y pulsa **Commit changes**.

### Paso 2.4. Activar GitHub Pages

1. En el repositorio, pulsa **Settings** (arriba).
2. En la columna izquierda, baja hasta **Pages** (sección *Code and automation*).
3. En **Source** elige **Deploy from a branch**.
4. En **Branch** selecciona `main` y en la carpeta de al lado deja `/ (root)`. Pulsa **Save**.
5. Espera **1 o 2 minutos** y recarga la página. Arriba aparecerá un recuadro verde con tu dirección.

### Paso 2.5. Tu dirección (URL) queda así

```
https://<usuario>.github.io/<repo>/
```

Con los ejemplos de arriba sería:

```
https://elcambiove.github.io/elcambio-privacidad/
```

**Reglas para construir la dirección:**

- `<usuario>` = tu nombre de usuario de GitHub, **en minúsculas**.
- `<repo>` = el nombre del repositorio, **en minúsculas**.
- Se usa `github.io` (no `github.com`), y siempre termina en `/`.

Si en cambio subiste la carpeta `privacidad` dentro de un repositorio existente llamado `dolar-venezuela`, la dirección sería:

```
https://<usuario>.github.io/dolar-venezuela/privacidad/
```

### Paso 2.6. Comprobar que funciona

1. Abre la dirección en una **ventana de incógnito** (para asegurarte de que cualquiera puede verla, sin iniciar sesión).
2. Ábrela también en tu **teléfono**: debe verse bien, sin necesidad de hacer zoom.
3. Comprueba que el **correo** y el **nombre** que escribiste aparecen correctamente (ya sin corchetes) y que el aviso azul del final ya no está.

---

## 3. Enlazarla en Google Play Console

1. Entra a `https://play.google.com/console` e inicia sesión.
2. Selecciona tu aplicación **ElCambio VE**.
3. En el menú de la izquierda busca **Contenido de la aplicación** (en inglés: *App content*).
   - En algunas versiones del panel el campo está en **Política y programas → Contenido de la aplicación → Política de privacidad**.
   - También puede aparecer en la ficha de la tienda, en **Presencia en la tienda → Ficha principal de la tienda → Política de privacidad**.
4. En el campo **Política de privacidad** pega tu dirección completa, empezando por `https://` (por ejemplo `https://elcambiove.github.io/elcambio-privacidad/`).
5. Pulsa **Guardar**.
6. Completa también el formulario **Seguridad de los datos** (*Data safety*): para eso te sirve la **sección 12 «Resumen para Google Play»** que está al final de la política, tanto en la página web como en `PRIVACY.md`. Resume exactamente qué se recopila, con qué finalidad, si se comparte y si es opcional.
7. Envía los cambios a revisión.

**Requisitos que debes cumplir (Google los revisa):**

- La dirección debe **abrirse sin iniciar sesión** y sin descargar nada. ✅ Una página de GitHub Pages cumple.
- **No** puede ser un PDF ni un documento de Google Drive: debe ser una página web. ✅ `index.html` lo es.
- Debe **mencionar la app por su nombre** y **decir qué datos se recopilan**. ✅ Ya lo hace.
- Debe incluir **un medio de contacto**. ✅ Es el correo que reemplazaste.
- La dirección debería **seguir siendo la misma** en el futuro (si la cambias, actualízala también en Play Console).

---

## 4. Cómo actualizarla después

Cuando cambies algo en la app o quieras corregir el texto:

1. **Edita el contenido.** Puedes hacerlo directamente en GitHub:
   - Entra a tu repositorio, haz clic en `index.html`.
   - Pulsa el **lápiz** (✏️ *Edit this file*).
   - Haz los cambios y pulsa **Commit changes**.
   - La web se actualiza sola en **1 o 2 minutos** (si no ves el cambio, recarga con `Ctrl + F5`).
   - Alternativa: vuelve a subir el archivo con **Add file → Upload files** (reemplaza el anterior).
2. **Actualiza la fecha.** En la parte de arriba de la página hay dos datos: *Entrada en vigor* (no la cambies) y *Última actualización* (ponla con la fecha del día). Cambia también la fecha al final de la sección 10 y en `PRIVACY.md`, para que los tres archivos digan lo mismo.
3. **Si el cambio es importante** (por ejemplo, si empezaras a recopilar un dato nuevo), avísalo en la ficha de la tienda o dentro de la app, y revisa que la sección 12 y el formulario de *Seguridad de los datos* sigan coincidiendo.
4. **Si cambias de dirección**, actualízala también en Google Play Console.

> **Consejo:** guarda siempre los cambios con un mensaje claro (`Commit changes`), así podrás ver el historial y volver atrás si algo sale mal.

---

## 5. Alternativa: usar tu propio hosting (sin GitHub)

Si ya tienes un dominio y hosting (por ejemplo con cPanel, Hostinger, GoDaddy, Donweb, etc.), puedes publicar ahí en lugar de GitHub Pages:

1. Abre el **administrador de archivos** de tu hosting (en cPanel se llama *Administrador de archivos* / *File Manager*).
2. Entra en la carpeta pública, normalmente `public_html` (a veces `www` o `htdocs`).
3. Crea una carpeta llamada `privacidad`.
4. Sube dentro el archivo `index.html` (botón **Upload** / **Subir**).
5. Tu dirección quedará así: `https://tudominio.com/privacidad/`
   - Si prefieres algo más corto, sube el archivo a `public_html` y cámbiale el nombre a `privacidad.html`. Entonces la dirección será `https://tudominio.com/privacidad.html`.
6. Comprueba que se abre en una ventana de incógnito y en el teléfono, y pega **esa** dirección en Play Console (paso 3).

**Otras opciones gratuitas equivalentes:** servicios como *Netlify Drop* o *Cloudflare Pages* permiten arrastrar el archivo `index.html` y publicarlo al instante; te dan una dirección propia que también puedes usar en Play Console.

Lo único que importa para Google Play es que la dirección sea **pública, sin inicio de sesión, en formato página web y con el nombre de la app y los datos recopilados dentro**.

---

## 6. Preguntas frecuentes

**¿Necesito saber programar?**
No. Solo reemplazar dos textos y subir un archivo.

**¿Cuánto cuesta?**
GitHub Pages es gratis.

**¿La página necesita internet para verse bien?**
No. Todo (el diseño, los colores, la letra) está dentro del mismo archivo `index.html`. Por eso se ve bien tanto en GitHub Pages como abierta en tu computadora sin conexión.

**¿Puedo usar la dirección de GitHub Pages si luego borro el repositorio?**
No. Si borras el repositorio o desactivas Pages, el enlace deja de funcionar y Google Play mostraría un error. Mantenlo publicado.

**¿La política guarda datos de quienes la visitan?**
No. La página no tiene formularios, ni cookies, ni contadores, ni publicidad; es solo texto con estilos.

---

## 7. Lista de verificación final

- [ ] Reemplacé `[NOMBRE DEL RESPONSABLE]` en `index.html` y en `PRIVACY.md`.
- [ ] Reemplacé `[CORREO DE CONTACTO]` en `index.html` y en `PRIVACY.md`.
- [ ] Borré el aviso azul del final de `index.html` y el comentario final de `PRIVACY.md`.
- [ ] Las fechas son iguales en los tres archivos (entrada en vigor y última actualización).
- [ ] Abrí la dirección en incógnito y en el teléfono, y se ve bien.
- [ ] Pegué la dirección en **Contenido de la aplicación → Política de privacidad** de Play Console.
- [ ] Completé el formulario **Seguridad de los datos** usando la sección 12 de la política.
