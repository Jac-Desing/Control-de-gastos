# App web modelo v22 Cloud

Versión corregida sobre la v21 cloud y la v19 funcional.

## Cambios v22

- Crea automáticamente el documento inicial en Firestore cuando el usuario entra por primera vez.
- Usa la ruta de nube: `users/{uid}/models/principal`.
- Si Firestore está vacío, carga el modelo base completo derivado del Excel original.
- Guarda el modelo como texto JSON para evitar el error de Firestore por arrays anidados.
- Valida que el modelo tenga períodos, secciones, gastos variables y bancos antes de usarlo.
- Migra datos locales previos desde v21/v20/v19 si existen.
- Evita que la app se quede indefinidamente en "Cargando nube...".
- Mantiene las funcionalidades de la v19/v21: formulario solo para gastos variables, meses ocultables, informe de inputs en Excel, comentarios por celda, paneles inmovilizados, resumen superior y lógica financiera del Excel.

## Reglas Firestore requeridas

Pegar en Firestore > Reglas y publicar:

```txt
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /users/{userId}/models/{modelId} {
      allow read, write: if request.auth != null && request.auth.uid == userId;
    }
  }
}
```

## Publicación

Subir `index.html` y `README.md` a GitHub Pages reemplazando la versión anterior.
