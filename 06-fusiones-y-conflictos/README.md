# 06 · Merge y conflictos en Git, paso a paso

## Resumen

- Merge: fast-forward o de 3 vías
- Conflicto = misma línea, dos cambios
- Resolver: elegir + add + commit

## Comandos de la lección

**Merge fast-forward**
```bash
git switch main
git merge nueva-portada
```

**Git avisa: CONFLICT** ⚠️ (cuidado)
```bash
git merge otra-rama
```

**Los marcadores de conflicto**
```text
<<<<<<< HEAD
<h1>Mi Web azul</h1>
=======
<h1>Mi Web verde</h1>
>>>>>>> otra-rama
```

**Resolver y cerrar el merge**
```bash
# 1. Edita el archivo y deja la versión buena
git add index.html
git commit -m "Resuelve el conflicto de la portada"
```

## Mini-reto

- Provoca un conflicto en index.html
- Resuélvelo con add + commit

<details><summary>Ver solución</summary>

```bash
git merge otra-rama
# editar index.html y quitar los marcadores
git add index.html
git commit -m "Resuelve el conflicto"
```
</details>

## Siguiente

➡️ [07 · GitHub: push, pull, fetch y clone](../07-repositorios-remotos/)
