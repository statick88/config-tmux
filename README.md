#  Configuración Personalizada de Tmux

Este repositorio contiene una configuración personalizada de **tmux** para mejorar la experiencia en la terminal con características como el soporte para plugins, la navegación estilo Vim, el uso del ratón, y una barra de estado personalizada. Además, incluye **Tmux Plugin Manager (TPM)** para facilitar la instalación y gestión de plugins.

## Requisitos

- tmux (versión 3.0 o superior recomendada)
- git (para clonar el repositorio)
- TPM (Tmux Plugin Manager) se incluye en esta configuración.

## Instalación
Para utilizar esta configuración en tu entorno local, sigue estos pasos:

1. Clona el repositorio y elimina el historial de Git para que puedas personalizarlo libremente sin arrastrar el historial del repositorio original:

```bash
git clone https://github.com/statick88/config-tmux.git ~/.tmux
rm -rf ~/.tmux/.git
```
2. Crear un enlace simbólico al archivo de configuración:

```bash
ln -s ~/.tmux/.tmux.conf ~/.tmux.conf
```
3. Instala los plugins usando Tmux Plugin Manager (TPM):

  1. Inicia una nueva sesión de tmux:

```bash
tmux
```

  2. Pulsa <kbd>Ctrl</kbd> + <kbd>x</kbd> (o el prefijo que hayas configurado) seguido de <kbd>I</kbd> (letra "i" mayúscula). Esto instalará automáticamente todos los plugins listados en el archivo .tmux.conf.

## Actualización de Plugins

Para actualizar los plugins, puedes usar el comando:

```bash
# Dentro de una sesión de tmux:
<Ctrl-x> + U
```
Esto actualizará todos los plugins instalados.

# Características Principales

- División de ventanas con atajos rápidos.

- Navegación estilo Vim entre paneles (h, j, k, l).

- Redimensionamiento fácil de paneles.

- Copia y pega usando el ratón o atajos.

- Barra de estado personalizable con información del sistema.

- Soporte para plugins gracias a TPM.

# Personalización

Para personalizar esta configuración, edita el archivo **~/.tmux/.tmux.conf** según tus preferencias.
