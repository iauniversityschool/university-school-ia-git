# 05 · Ramas en Git: branch y switch

## Resumen

- Rama = línea del tiempo paralela
- branch crea · switch cambia · -c ambas
- HEAD = dónde estás parado

## Comandos de la lección

**Ver y crear ramas**
```bash
git branch
git branch nueva-portada
```

**Cambiar (y crear + cambiar)**
```bash
git switch nueva-portada

# crear y cambiar en un paso:
git switch -c otra-rama
```

**Commit en la rama nueva**
```bash
echo "<h2>Nueva portada</h2>" > portada.html
git add portada.html
git commit -m "Añade la nueva portada"
```

**Volver a main**
```bash
git switch main
ls
```

## Mini-reto

- Crea la rama 'prueba' y haz un commit
- Vuelve a main y revisa con git branch

<details><summary>Ver solución</summary>

```bash
git switch -c prueba
git commit -am "Cambio de prueba"
git switch main
git branch
```
</details>

## Siguiente

➡️ [06 · Merge y conflictos en Git, paso a paso](../06-fusiones-y-conflictos/)
