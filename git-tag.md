# git tag
Lista las etiquetas en orden alfabetico.

## git tag -a nombre_etiqueta -m "mensaje de la etiqueta"
Etiqueta anotada. Se guarda en la base de datos de git como un objeto de entero. Tiene un checksum, correo electronico y tiene fecha; y tiene un mensaje asociado.

```
git tag -l "v1.*"
```
Lista de las etiquetas que concidan con el patron especificado.