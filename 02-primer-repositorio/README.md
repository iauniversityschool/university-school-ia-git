# 02 · Tu primer repositorio: init, add, commit

## Resumen

Git tiene **tres zonas**:

1. **Directorio de trabajo** — tus archivos tal como los editas.
2. **Staging area** — la "sala de espera"; eliges qué cambios guardar (como el carrito del súper).
3. **Repositorio** — donde quedan los `commit` para siempre.

El ciclo es siempre: editar → `git add` (al staging) → `git commit` (al repositorio).

## Comandos

Crear el repositorio:
```bash
mkdir mi-web
cd mi-web
git init
```

Ver el estado (tu brújula):
```bash
git status
```

El ciclo add → commit:
```bash
echo "<h1>Mi Web</h1>" > index.html
git add index.html
git commit -m "Crea la página de inicio"
```

Ver el historial:
```bash
git log --oneline
```

## Buenos mensajes de commit

- 📏 Cortos y claros.
- 🎯 Di **qué** hace el cambio, no cómo.
- ▶️ En presente, como una orden: `Añade`, `Corrige`, `Elimina`.

## Mini-reto

Crea `sobre.html`, añádelo y haz un commit con un buen mensaje:
```bash
echo "<h1>Sobre mí</h1>" > sobre.html
git add sobre.html
git commit -m "Añade la página sobre mí"
```

## Siguiente

➡️ [03 · Ignorar archivos con .gitignore](../03-gitignore/)
