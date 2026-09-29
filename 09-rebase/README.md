# 09 · Rebase en Git: historia limpia

## Resumen

- Rebase = historia en línea recta
- Interactivo: squash, reword, reordenar
- ⚠️ Nunca rebase de lo ya compartido

## Comandos de la lección

**Poner tu rama al día**
```bash
git switch mi-rama
git rebase main
```

**git rebase -i HEAD~3**
```text
pick   a1b2c3d  Primer intento
squash e4f5g6h  Arreglo rápido
squash 7h8i9j0  Otro arreglo
```

**Tres commits → uno limpio**
```bash
git log --oneline
```

### merge vs rebase

| 🔀 merge | 📏 rebase |
|---|---|
| Historia real, con curvas | Historia en línea recta |
| Añade commit de merge | Sin commits extra |
| Fiel a lo que pasó | Más fácil de leer |

## Mini-reto

- Haz 3 commits y únelos en 1
- git rebase -i HEAD~3 + squash

<details><summary>Ver solución</summary>

```bash
git rebase -i HEAD~3
# dejar 'pick' en el 1º, 'squash' en los otros dos
git log --oneline
```
</details>

## Siguiente

➡️ [10 · Git stash: guardar trabajo a medias](../10-stash/)
