# 03 · Ignorar archivos con .gitignore

## Resumen

No todo debe entrar en Git. El archivo **`.gitignore`** le dice a Git qué archivos ignorar.

**Qué NO versionar:**
- 🔒 **Secretos:** `.env`, claves de API, contraseñas.
- 📦 **Dependencias reinstalables:** `node_modules/`.
- 🗑️ **Temporales o generados:** `*.log`, `build/`.

## El archivo .gitignore

Créalo en la raíz del proyecto (empieza con un punto, sin nombre antes). Una regla por línea:
```
.env
node_modules/
*.log
```

### Patrones

| Patrón | Ignora |
|--------|--------|
| `.env` | ese archivo exacto |
| `node_modules/` | toda esa carpeta |
| `*.log` | todos los archivos que terminan en `.log` |
| `temp/*` | todo lo que hay dentro de `temp` |

## Trampa común: algo ya rastreado

`.gitignore` solo ignora archivos que Git **aún no rastrea**. Si un archivo ya lo guardaste en un commit, sácalo del rastreo (queda en tu disco):
```bash
git rm --cached secretos.env
git commit -m "Deja de rastrear secretos.env"
```

## Truco: no empieces de cero

La web [gitignore.io](https://www.toptal.com/developers/gitignore) genera un `.gitignore` listo según tu lenguaje o sistema (Node, Python, Windows, Mac…). Copia y pega.

## Mini-reto

Crea un `.gitignore` que ignore todos los `.log` y la carpeta `temp/`:
```
*.log
temp/
```

## Siguiente

➡️ [04 · Deshacer cambios: restore, reset y amend](../04-deshacer-cambios/)
