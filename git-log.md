### git log
Muestra todo el historial de commits del proyecto.

```
git log
git log --oneline --graph
git lop -2
git log --pretty=format:"%h - %an,%ar : %s"
```
Muestra el historial en el formato que indicamos

```
git log --after="2017-11-25 00:00:00"
git log --before="2017-11-25 00:00:00"
git log --after="2017-11-24 16:00:00" --before="2017-11-24 19:00:00"

`git log --oneline`
Este comando nos muestra el historial en una sola linea por commit.
