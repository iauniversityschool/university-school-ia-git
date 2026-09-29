# 01 · Instalación y configuración (Windows, macOS, Linux)

## Resumen

Instala Git en cualquier sistema y preséntate con tu nombre y correo. Cada `commit` llevará esa firma. Se configura una sola vez.

## Instalar Git

**Windows:** descarga el instalador desde [git-scm.com](https://git-scm.com) y ábrelo. Deja las opciones por defecto (siguiente → instalar). Incluye la terminal **Git Bash**.

**macOS (con [Homebrew](https://brew.sh)):**
```bash
brew install git
```

**Linux (Ubuntu / Debian):**
```bash
sudo apt install git
```

**Linux (Fedora):**
```bash
sudo dnf install git
```

Comprueba la instalación:
```bash
git --version
```

## Configurar tu identidad

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tucorreo@ejemplo.com"
git config --global init.defaultBranch main
```

- `--global` = vale para todos tus proyectos.
- Usa el mismo correo que usarás en GitHub.
- `init.defaultBranch main` hace que la rama principal se llame `main`.

Revisa todo:
```bash
git config --list
```

## Clave SSH (para conectar con GitHub sin contraseña)

```bash
ssh-keygen -t ed25519 -C "tucorreo@ejemplo.com"
```

Pulsa Enter en cada pregunta. Luego copia la clave **pública** (archivo terminado en `.pub`) y pégala en GitHub → **Settings → SSH and GPG keys**.

## Mini-reto

Configura tu nombre y tu correo, y verifícalo:
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tucorreo@ejemplo.com"
git config --list
```

## Siguiente

➡️ [02 · Tu primer repositorio](../02-primer-repositorio/)
