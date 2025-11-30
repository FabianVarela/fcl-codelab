### Paso 1: Exportar el archivo Markdown con claat

Primero, exporté el archivo Markdown del codelab usando el comando claat export:
```bash
claat export codelabs/data-connect-flutter.md
```

Explicación:
- claat export: Comando para convertir un archivo Markdown a HTML.
- -o /site: Especifica el directorio de salida en el que se generará el directorio del codelab.
- El último parámetro es la ruta al archivo de Markdown de origen.

Resultado:
Este comando creó/actualizó el folder data-connect-flutter/ con:
- codelab.json - metadata del codelab
- index.html - el contenido HTML generado
- img/ - folder con las imágenes

### Paso 2: Ejecutar el servidor con gulp

Finalmente, ejecuté el servidor de desarrollo:
```dart
cd /site && gulp serve
```

Resultado:
El servidor quedó corriendo y disponible en http://localhost:8000.
