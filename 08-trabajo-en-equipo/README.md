# 08 · Fork y Pull Requests: colaborar en GitHub

## Resumen

- Fork = tu copia del proyecto ajeno
- upstream = original · origin = tu fork
- Pull Request = propuesta que se revisa

## Comandos de la lección

**Seguir al original**
```bash
git remote add upstream git@github.com:autor/proyecto.git
git fetch upstream
```

### La revisión (code review)

| ✅ Aprobado | 🔁 Pide cambios |
|---|---|
| El revisor hace merge | Corriges y vuelves a subir |
| Tu cambio entra | El PR se actualiza solo |

## Mini-reto

- Ordena los pasos para contribuir
- Desde el fork hasta el Pull Request

<details><summary>Ver solución</summary>

- 1 · Fork  ·  2 · Clone
- 3 · Rama + commits  ·  4 · Push
- 5 · Pull Request  ·  6 · Revisión → merge
</details>

## Siguiente

➡️ [09 · Rebase en Git: historia limpia](../09-rebase/)
