# Angular Video Gallery con Firebase

Este proyecto en Angular se conecta a Firebase Firestore para mostrar una galería de videos musicales. Los usuarios pueden filtrar los videos por instrumento, categoría, orden alfabético o búsqueda por título. Los videos se muestran en un reproductor embebido.

---

## Características

-  Integración en tiempo real con Firebase Firestore
-  Filtros:
   -  Por instrumento
   - Por categoría musical
   - Orden alfabético (A-Z)
   - Búsqueda por texto
- Reproductor embebido (YouTube)
- Arquitectura Angular modular con componentes y servicios

---

##  Tecnologías

- Angular
- Firebase / Firestore
- AngularFire
- RxJS
- Bootstrap o TailwindCSS (opcional)

---

## Estructura del proyecto

```

src/
├── app/
│   ├── components/
│   │   ├── video-list/
│   │   └── video-card/
│   ├── services/
│   │   └── video.service.ts
│   ├── pipes/
│   │   └── safe-url.pipe.ts
│   ├── app.component.ts
│   └── app.module.ts

````

---

## Configuración

### 1. Clona el repositorio

```bash
git clone https://github.com/tuusuario/angular-firebase-videos.git
cd angular-firebase-videos
````

### 2. Instala dependencias

```bash
npm install
```

### 3. Configura Firebase

Crea un archivo `src/environments/environment.ts` con tu configuración de Firebase:

```ts
export const environment = {
  production: false,
  firebase: {
    apiKey: 'TU_API_KEY',
    authDomain: 'TU_DOMINIO.firebaseapp.com',
    projectId: 'TU_PROJECT_ID',
    storageBucket: 'TU_BUCKET',
    messagingSenderId: 'TU_SENDER_ID',
    appId: 'TU_APP_ID'
  }
};
```

> También asegúrate de activar **Firestore Database** en la consola de Firebase.

---

### 4. Ejecuta el servidor local

```bash
ng serve
```

Abre `http://localhost:4200` para ver la app.

---

## Estructura de datos en Firestore

**Colección:** `videos`

**Documento de ejemplo:**

```json
{
  "title": "Piano Jazz Improvisation",
  "category": "Jazz",
  "instrument": "Piano",
  "videoUrl": "https://www.youtube.com/embed/XYZ123",
  "createdAt": "2024-01-01T12:00:00Z"
}
```

---

## 📸 Capturas de pantalla

> Puedes agregar capturas del listado de videos, los filtros en acción, etc.

---

## Contribuciones

Las contribuciones son bienvenidas.
Haz un fork del proyecto y envía un pull request. ¡Gracias por ayudar!

---

##  Licencia

Este proyecto está bajo la licencia MIT.

---

## 👩‍💻 Autor

Desarrollado por **\Neydaris Puentes**
GitHub: [@neydarisJaylinne](https://github.com/neydarisJaylinne)
