# 17 · Proyecto final: el flujo completo de Git

## Resumen

- De cero al flujo profesional completo
- Practica en tus proyectos reales
- ¡Suscríbete para el próximo curso!

## Comandos de la lección

**Paso 1: iniciar el proyecto**
```bash
git init
echo "node_modules/" > .gitignore
git add .
git commit -m "chore: inicia el proyecto mi-web"
```

**Paso 2: rama de funcionalidad**
```bash
git switch -c feature-galeria
# ... editar archivos ...
git commit -am "feat: añade la galería de fotos"
```

**Paso 3: push y Pull Request**
```bash
git push -u origin feature-galeria
# abrir el Pull Request en GitHub
```

**Paso 4: merge, tag y release**
```bash
git switch main
git pull
git tag -a v1.0.0 -m "Primera versión"
git push origin v1.0.0
```

## Mini-reto

- Reproduce el flujo completo en tu repo
- init → rama → commits → merge → tag

## ¡Fin del curso!

Practica el flujo completo en tus propios proyectos. Suscríbete a University School IA para el próximo curso.
