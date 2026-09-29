# 07 · GitHub: push, pull, fetch y clone

## Resumen

- origin = tu repo en la nube
- push sube · pull baja · clone copia todo
- pull = fetch + merge

## Comandos de la lección

**Conectar tu repo**
```bash
git remote add origin git@github.com:usuario/mi-web.git
git remote -v
```

**Subir con push**
```bash
git push -u origin main
```

**Clonar un repo existente**
```bash
git clone git@github.com:usuario/mi-web.git
```

**Bajar lo último**
```bash
git pull
```

### fetch vs pull

| ⬇️ fetch | ⬇️ pull |
|---|---|
| Baja los cambios | Baja los cambios |
| No los aplica | Y los fusiona |
| Solo mirar | pull = fetch + merge |

## Mini-reto

- Sube mi-web a un repo nuevo de GitHub
- remote add origin → push -u origin main

<details><summary>Ver solución</summary>

```bash
git remote add origin git@github.com:usuario/mi-web.git
git push -u origin main
```
</details>

## Siguiente

➡️ [08 · Fork y Pull Requests: colaborar en GitHub](../08-trabajo-en-equipo/)
