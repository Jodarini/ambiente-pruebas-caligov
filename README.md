# Ambiente de Pruebas para Micrositios de Cali.gov.co

## Descripción

Este repositorio proporciona un entorno local para agilizar el desarrollo y previsualización de micrositios para Cali.gov.co. Elimina la necesidad de:

- Esperar a que los servidores de cali.gov.co respondan
- Usar el editor de publicaciones del CMS oficial
- Publicar cambios solo para previsualizarlos

Con esta solución, los cambios se reflejan al instante al guardar los archivos.

## Características Principales

- ⚡ Recarga instantánea - Cambios visibles inmediatamente
- ✏ Entorno de edición focalizado - Solo edita lo que tendrías en el CMS real
- 🛠 Fiel al entorno de producción - Mismo comportamiento que el CMS oficial
- 📁 Estructura simple - Fácil de entender y usar

## Requisitos Previos

- Node.js (v18+ recomendado)
- pnpm (alternativamente npm o yarn)

## Configuración Inicial
1. Clona el repositorio:

        git clone https://github.com/Jodarini/ambiente-pruebas-caligov.git
        cd ambiente-pruebas-caligov


2. Instala las dependencias:

        pnpm install

3. Inicia el servidor de desarrollo:

        pnpm run dev

4. Abre tu navegador en http://localhost:5173

## Flujo de Trabajo
- Edita solo main.js - Este es el único archivo que modificarías en el CMS real
- Guarda los cambios - La página se recargará automáticamente
- Previsualiza - Ve los cambios al instante en tu navegador

## Estructura del Proyecto

    ├── public/              # Archivos estáticos (simulan el CMS)
    ├── src/
    │   └── main.js          # Único archivo a editar (simula la entrada del CMS)
    ├── index.html           # Página contenedora
    └── vite.config.js       # Configuración del servidor de desarrollo

## Limitaciones
- Este entorno solo simula el comportamiento del CMS para fines de desarrollo
- Algunas funcionalidades que dependen de servicios backend de cali.gov.co podrían no estar disponibles
- El diseño final puede variar ligeramente del entorno de producción

## Contribuciones

Las contribuciones son bienvenidas. Por favor abre un issue o pull request para:
- Reportar errores
- Sugerir mejoras
- Agregar nuevas funcionalidades

Nota: Recuerda que este es solo un entorno de desarrollo. Los cambios finales deben ser implementados a través del CMS oficial de Cali.gov.co.
