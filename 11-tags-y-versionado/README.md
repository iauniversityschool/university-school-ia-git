# 11 · Tags y versionado: releases y SemVer

## Resumen

- Tag anotado marca la versión
- SemVer: MAJOR.MINOR.PATCH
- push origin <tag> → Release en GitHub

## Comandos de la lección

**Crear un tag anotado**
```bash
git tag -a v1.0.0 -m "Primera versión estable"
git tag
```

**Subir el tag a GitHub**
```bash
git push origin v1.0.0
```

### Ligero vs anotado

| 🏷️ Ligero | 📌 Anotado |
|---|---|
| Solo un nombre | Nombre + autor + fecha |
| Rápido | Lleva un mensaje |
| Para uso interno | Para publicar |

## Mini-reto

- Crea el tag anotado v1.0.0
- Súbelo con git push origin v1.0.0

<details><summary>Ver solución</summary>

```bash
git tag -a v1.0.0 -m "Primera versión estable"
git push origin v1.0.0
```
</details>

## Siguiente

➡️ [12 · diff, log, blame y cherry-pick](../12-inspeccionar-historial/)
