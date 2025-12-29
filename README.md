# Bun AI API

Este proyecto es una API construida con [Bun](https://bun.sh) que integra servicios de IA como Groq y Cerebras.

## Requisitos Previos

El único requisito principal para ejecutar este proyecto es tener **Bun** instalado en tu sistema.

### ¿No tienes Bun instalado?

Si aún no tienes Bun, puedes instalarlo siguiendo las instrucciones oficiales o ejecutando el siguiente comando en tu terminal (para macOS, Linux y WSL):

```bash
curl -fsSL https://bun.sh/install | bash
```

Para usuarios de Windows, se recomienda usar WSL o seguir las instrucciones específicas en su página web.

👉 [Visita la página oficial de Bun para más detalles](https://bun.sh)

## Configuración e Instalación

Sigue estos pasos detallados para poner en marcha el proyecto:

### 1. Instalar dependencias

Una vez clonado el proyecto, abre tu terminal en la carpeta raíz del proyecto y ejecuta:

```bash
bun install
```

Este comando descargará e instalará todas las librerías necesarias listadas en el archivo `package.json`.

### 2. Configurar Variables de Entorno

El proyecto necesita ciertas claves de API para funcionar. Debes crear un archivo para almacenarlas de forma segura.

1.  Crea un archivo llamado `.env` en la raíz del proyecto.
2.  Abre el archivo `.env` y añade las siguientes variables (reemplaza los valores de ejemplo con tus propias claves reales):

```env
# Puerto del servidor (opcional, por defecto 3000)
PORT=3000

# API Key para el servicio de Groq
GROQ_API_KEY=gsk_...

# API Key para el servicio de Cerebras
CEREBRAS_API_KEY=csk_...
```

**Nota:** Asegúrate de obtener tus API Keys en los portales de desarrollador de Groq y Cerebras respectivamente.

### 3. Ejecutar el Proyecto

Tienes dos formas de ejecutar el servidor, dependiendo de si estás desarrollando o quieres ejecutarlo en producción.

#### Modo Desarrollo (`dev`)

Este modo es ideal mientras estás editando código, ya que reinicia el servidor automáticamente cuando guardas cambios (`--watch` mode).

```bash
bun run dev
```

#### Modo Producción (`start`)

Utiliza este comando para una ejecución estable sin reinicios automáticos.

```bash
bun run start
```

Verás un mensaje en la consola indicando que el servidor está corriendo, por ejemplo:
`Server is running on http://localhost:3000`

## Tutorial

Mira el video explicativo de cómo se ha creado este proyecto:


[![Video Tutorial](https://img.youtube.com/vi/ax7_QNZZ-pk/0.jpg)](https://www.youtube.com/watch?v=ax7_QNZZ-pk)
