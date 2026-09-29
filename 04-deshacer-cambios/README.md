# 04 · Deshacer cambios: restore, reset y amend

## Resumen

- restore: descartar / sacar del staging
- commit --amend: corregir el último
- reset: soft y mixed seguros, hard borra

## Comandos de la lección

**Descartar cambios del archivo**
```bash
git restore index.html
```

**Sacar del staging**
```bash
git restore --staged index.html
```

**git commit --amend**
```bash
git commit --amend -m "Mensaje corregido"
```

**Ejemplo seguro: --soft**
```bash
git reset --soft HEAD~1
```

**Peligroso: --hard borra cambios** ⚠️ (cuidado)
```bash
git reset --hard HEAD~1
```

### Los tres modos de reset

| ✅ Seguros | ⚠️ Peligroso |
|---|---|
| --soft: cambios al staging | --hard: borra los cambios |
| --mixed: cambios al trabajo | No hay papelera obvia |

## Mini-reto

- Añade un cambio al staging y sácalo
- Sin perder el cambio (--staged)

<details><summary>Ver solución</summary>

```bash
git add index.html
git restore --staged index.html
git status
```
</details>

## Siguiente

➡️ [05 · Ramas en Git: branch y switch](../05-ramas/)
