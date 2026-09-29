# 10 · Git stash: guardar trabajo a medias

## Resumen

- Stash = cajón para cambios a medias
- stash guarda · list ve · pop recupera
- pop borra el stash · apply lo conserva

## Comandos de la lección

**Guardar en el cajón**
```bash
git stash
```

**Ver el cajón**
```bash
git stash list
```

**Recuperar con pop**
```bash
git stash pop
```

### pop vs apply

| 📤 pop | 📋 apply |
|---|---|
| Recupera los cambios | Recupera los cambios |
| Borra el stash | Conserva el stash |
| El caso normal | Para reutilizarlo |

## Mini-reto

- Guarda un cambio con git stash
- Comprueba que el árbol quedó limpio

<details><summary>Ver solución</summary>

```bash
git stash
git status
git stash pop
```
</details>

## Siguiente

➡️ [11 · Tags y versionado: releases y SemVer](../11-tags-y-versionado/)
