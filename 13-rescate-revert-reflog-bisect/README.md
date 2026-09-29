# 13 · Rescate en Git: revert, reflog y bisect

## Resumen

- revert: deshacer sin borrar historia
- reflog: la papelera de Git
- bisect: caza el commit culpable

## Comandos de la lección

**git revert <hash>**
```bash
git revert e4f5g6h
```

**Ver el reflog**
```bash
git reflog
```

**Recuperar lo perdido**
```bash
git reset --hard 53c0019
```

**Empezar la búsqueda**
```bash
git bisect start
git bisect bad
git bisect good a1b2c3d
```

**Encontrar al culpable**
```bash
git bisect bad
# ... hasta que Git lo encuentra
git bisect reset
```

### revert vs reset

| ⏪ reset | ↩️ revert |
|---|---|
| Borra commits | Crea un commit que deshace |
| Reescribe la historia | Conserva la historia |
| Peligroso si compartido | Seguro en equipo |

## Mini-reto

- Borra un commit con reset --hard
- Recupéralo con git reflog

<details><summary>Ver solución</summary>

```bash
git reflog
git reset --hard 53c0019
```
</details>

## Siguiente

➡️ [14 · Flujos de trabajo: GitHub Flow, Git Flow y trunk-based](../14-flujos-de-trabajo/)
