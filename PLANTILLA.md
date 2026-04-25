# 🛠️ Guía de Configuración: [PROYECTO]-desktop-electron

> **¡Atención!** Si acabas de clonar este repositorio para un nuevo proyecto, sigue esta guía técnica para estandarizar tu entorno. Una vez finalices, **elimina este archivo**.

---

### 📦 1. Identidad y Nomenclatura (package.json)

Es vital mantener la convención profesional de nombres para asegurar el orden en el ecosistema.

| Atributo | Formato Requerido | Ejemplo |
| :--- | :--- | :--- |
| **Repo Name** | `[proyecto]-[plataforma]-[tipo]` | `yachakuy-desktop-electron` |
| **Property "name"** | Mismo nombre del repositorio | `"yachakuy-desktop-electron"` |

**Acciones:**
* Actualiza el campo `"name"` con el patrón indicado.
* Modifica los metadatos: `"description"`, `"version"`, `"author"`.

---

### 🌐 2. Conexión de Capas (main.js)

Vincula este contenedor con tu aplicación web principal.

* **Punto de Entrada:** Cambia la constante `APP_URL`.
    * *Local:* `http://yachakuy.test`
    * *Producción:* `https://yachakuy.com`
* **Viewport:** Ajusta `width` y `height` según la resolución mínima recomendada para tu aplicación.

---

### 🎨 3. Identidad Visual (Branding)

1.  Crea el directorio `/public` en la raíz.
2.  Agrega el logo de la aplicación con la siguiente nomenclatura:
    * `icon.ico` para sistemas Windows.
    * `icon.png` para sistemas Linux/Mac.
3.  **Activa el ícono:** En `main.js`, busca y descomenta la línea que define el atributo `icon:`.

---

### 📝 4. Documentación Final (README.md)

El archivo `README.md` es la cara de tu proyecto. 
* Reemplaza todos los textos entre corchetes `[ ]` con la información real del producto.
* Asegúrate de que los enlaces y nombres reflejen el nuevo dominio del proyecto.

---

### 🧹 5. Finalización y Primer Commit

Una vez completados los pasos anteriores, limpia el repositorio para el primer despliegue:

1.  **Elimina este archivo:** `rm PLANTILLA.md`
2.  **Sincroniza dependencias:** `npm install`
3.  **Commit de inicialización:**
    ```bash
    git add .
    git commit -m "build: project start [proyecto]-desktop-electron"
    ```

---
**¡Listo!** El contenedor está configurado bajo los estándares de la industria. 🚀