### git log

Muestra todo el historial de commits del proyecto

```
git log --pretty=format:"%h - %an, %ar : %s"
```

Muestra el historial con el formato indicado, en este caso:

1. `%h` - Hash en formato abreviado
2. `%an` - Nombre del autor de cada commit que se encuentre
3. `%ar` - Fecha de autoría relativa
4. `%s` - Asunto del commit (título)

#### Limitar la salida del historial

`git log --after="2018-02-07 00:00:00"`: Muestra los commits realizados después de la fecha especificada.

`git log --before="2018-02-08 00:00:00"`: Muestra los commits realizados antes de la fecha especificada.

Las banderas del comando `git log`se pueden usar juntas según convenga, por ejemplo:
`git log --after="2018-02/07 12:00:00" --before="2018-04-07 12:30:00"`

