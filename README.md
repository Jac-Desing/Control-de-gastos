# App web modelo v20

Versión basada en la v19, con sincronización en la nube mediante Firebase Authentication y Cloud Firestore.

## Funciones principales

- Un solo modelo sincronizado por usuario.
- Inicio de sesión con correo y contraseña.
- Guardado automático en Firestore.
- Respaldo local en el navegador.
- Conserva las funcionalidades de la v19: meses ocultables, formulario solo para gastos variables, comentarios por celda, informe Excel, conceptos editables, paneles inmovilizados y lógica del Excel original.

## Reglas sugeridas de Firestore

Pegar en Firestore > Reglas:

```
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /users/{userId}/models/{modelId} {
      allow read, write: if request.auth != null && request.auth.uid == userId;
    }
  }
}
```

## Nota de migración

Si el navegador tenía datos de la v19, la v20 intenta leerlos desde el almacenamiento local anterior y subirlos como primer modelo en la nube al crear/iniciar sesión.
