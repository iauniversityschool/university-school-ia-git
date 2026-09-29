# 15 · Conventional Commits, hooks y alias

## Resumen

- Conventional Commits: feat, fix, docs…
- Hooks: automatiza (pre-commit)
- Alias: tus propios atajos

## Comandos de la lección

**El formato**
```bash
git commit -m "feat: añade el formulario de contacto"
git commit -m "fix: corrige el enlace roto del menú"
```

**Un hook pre-commit**
```bash
#!/bin/sh
npm test
```

**Crear alias**
```bash
git config --global alias.lg "log --oneline --graph --all"
git config --global alias.st "status"
```

## Mini-reto

- Un commit 'feat: ...'
- Un alias 'lg' para el log en grafo

<details><summary>Ver solución</summary>

```bash
git commit -m "feat: añade la galería de fotos"
git config --global alias.lg "log --oneline --graph --all"
```
</details>

## Siguiente

➡️ [16 · Submódulos, worktrees, Git LFS y firmar commits](../16-extra-pro/)
