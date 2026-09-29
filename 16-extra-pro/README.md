# 16 · Submódulos, worktrees, Git LFS y firmar commits

## Resumen

- Submódulo: repo dentro de repo
- Worktree: varias ramas a la vez
- LFS: archivos grandes · -S: firmar

## Comandos de la lección

**Añadir un submódulo**
```bash
git submodule add git@github.com:autor/libreria.git
```

**Crear un worktree**
```bash
git worktree add ../revision pull-request-42
```

**Rastrear archivos grandes**
```bash
git lfs install
git lfs track "*.mp4"
```

**Firmar = insignia 'Verified'**
```bash
git commit -S -m "feat: añade el login"
```

## Mini-reto

- 1 · Librería externa con su historia
- 2 · Videos pesados en el repo
- 3 · Revisar un PR sin parar tu trabajo

<details><summary>Ver solución</summary>

- 1 · Librería externa → Submódulo
- 2 · Videos pesados → Git LFS
- 3 · Revisar un PR aparte → Worktree
</details>

## Siguiente

➡️ [17 · Proyecto final: el flujo completo de Git](../17-proyecto-final/)
