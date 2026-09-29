# 12 · diff, log, blame y cherry-pick

## Resumen

- diff: qué cambió · log --graph: el árbol
- blame: quién escribió cada línea
- cherry-pick: un commit suelto

## Comandos de la lección

**git diff: qué cambió**
```diff
  <h1>Mi Web</h1>
- <p>Hola</p>
+ <p>Bienvenido</p>
```

**git log como un mapa**
```bash
git log --oneline --graph --all
```

**git blame archivo**
```bash
git blame index.html
```

**git cherry-pick <hash>**
```bash
git cherry-pick e4f5g6h
```

## Mini-reto

- Mira un cambio con git diff
- Explora la historia con log --graph

<details><summary>Ver solución</summary>

```bash
git diff
git log --oneline --graph --all
```
</details>

## Siguiente

➡️ [13 · Rescate en Git: revert, reflog y bisect](../13-rescate-revert-reflog-bisect/)
