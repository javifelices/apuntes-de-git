### git log

Muestra el historial de commits

```
git log --pretty=format:"%h - %an, %ar : %s"
```

Muestra el historial con el formato indicado, en este caso:

1. `%h` - Hash en formato abreviado
2. `%an` - Nombre del autor de cada commit que se encuentre
3. `%ar` - Fecha de autoría relativa
4. `%s` - Asunto del commit (título)
