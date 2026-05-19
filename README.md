## 1. Validación de HTML y CSS con la W3C

La **W3C (World Wide Web Consortium)** es la organización internacional que desarrolla los estándares para la web. Como ya tenéis vuestros proyectos desplegados en **GitHub Pages**, utilizaremos el método de validación por URL fija. Cada vez que hagáis un `git push` y se actualice vuestra web, podréis volver a comprobar la URL.

### 🔍 Cómo validar tu HTML por URL
1. Entra en el [Validador de HTML de la W3C](https://validator.w3.org/).
2. Asegúrate de estar en la pestaña **"Validate by URI"**.
3. En el campo *Address*, pega la URL completa de tu GitHub Pages (ej. `https://tu-usuario.github.io/tu-repositorio/`).
4. Haz clic en **Check**.
   
<img width="1588" height="407" alt="Group 41" src="https://github.com/user-attachments/assets/c47d6e1f-d542-41c9-a7e3-38630d7b0749" />

<img width="1588" height="723" alt="image 4" src="https://github.com/user-attachments/assets/760af8b9-f88a-4913-96de-150d121eff91" />

> 💡 **En qué fijarse:** Los *Errors* (en rojo) deben corregirse obligatoriamente, ya que rompen la estructura o la semántica. Los *Warnings* (en amarillo) son sugerencias de buenas prácticas o avisos sobre elementos redundantes que conviene revisar.

### 🎨 Cómo validar tu CSS por URL
1. Entra en el [Validador de CSS de la W3C](https://jigsaw.w3.org/css-validator/).
2. En la pestaña **"Por URL"**, introduce la misma dirección de tu GitHub Pages.
3. Haz clic en **Examinar**. Si la sintaxis de tus hojas de estilo es correcta, verás un mensaje de felicitación sobre fondo verde.

<img width="1588" height="407" alt="Group 42" src="https://github.com/user-attachments/assets/41edfa8b-177e-4f04-b7b7-c2d632047399" />

<img width="1588" height="521" alt="image 5" src="https://github.com/user-attachments/assets/e0bd5c2a-6196-4550-8cf0-0a6a56164359" />

---

## 2. ¿Qué pasa con JavaScript? (El concepto de Linting)

A diferencia de HTML y CSS, **JavaScript no tiene un validador oficial de la W3C** porque es un lenguaje de programación imperativo. Los errores graves de ejecución los veréis directamente en la consola del navegador, pero para evaluar la calidad del código utilizaremos una alternativa online:

1. Entra en [JSHint.com](https://jshint.com/).
2. Copia el código de tus archivos `.js` y pégalo en el editor de la izquierda.
3. En el panel de la derecha verás al instante advertencias sobre variables no declaradas, puntos y coma faltantes o malas prácticas estructurales.

---

## 3. Auditoría de Calidad Completa con Google Lighthouse

**Lighthouse** es una herramienta automatizada de Google integrada en Chrome que analiza el sitio web real y público. Al ejecutarlo sobre vuestra URL de GitHub Pages, evaluará cómo responde la web en un entorno de servidor real.

### 🛠️ Cómo pasar la auditoría:
1. Abre una ventana en **modo incógnito** en Google Chrome (esto evita que tus extensiones afecten a las puntuaciones de rendimiento).
2. Entra en la URL de tu **GitHub Pages**.
3. Abre las Herramientas de Desarrollador pulsando `F12` (o clic derecho -> *Inspeccionar*).
   
<img width="1588" height="894" alt="Group 44" src="https://github.com/user-attachments/assets/ca10ab4c-2d4c-49b9-bf39-03792d1f995a" />

5. En el menú de pestañas superior, selecciona **Lighthouse** (si no aparece a primera vista, haz clic en las flechas `>>`).

<img width="1588" height="894" alt="Group 45" src="https://github.com/user-attachments/assets/dda1e8cf-5818-44ea-a575-331c55936625" />

7. Configura la prueba:
   * **Mode:** Navigation (Default)
   * **Device:** Mobile (es el estándar de la industria, si pasa en móvil, pasará en escritorio).
8. Haz clic en **Analyze page load** y no toques la ventana hasta que termine.

<img width="1588" height="1638" alt="Group 46" src="https://github.com/user-attachments/assets/81ce93d8-b6d5-48b3-a123-86c61b56791e" />

### 🎯 Criterios de aceptación para la entrega
Para que la práctica esté aprobada, la última versión desplegada en vuestro repositorio debe cumplir:
* **HTML de la W3C:** 0 Errores.
* **CSS de la W3C:** 0 Errores.
* **Lighthouse:** Una puntuación superior a **90 puntos** (color verde) en las secciones de **Accesibilidad**, **Buenas Prácticas** y **SEO**.
