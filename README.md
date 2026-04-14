# 🎮 Gamepedia - Frontend II (Semana 6)

Este repositorio contiene la actividad práctica de la Semana 6 para la asignatura de Desarrollo Frontend II. El proyecto consiste en una plataforma de catálogo de videojuegos que implementa patrones avanzados de manejo de estado y automatización de procesos.

## 🚀 Características del Proyecto

* **Gestión de Estado Global:** Implementación de la API de Contexto de React para el manejo de la lista de Favoritos.
* **Navegación Dinámica:** Uso de `react-router-dom` para la gestión de rutas, incluyendo vistas de detalles de juegos basadas en parámetros de URL.
* **Consumo de API:** Integración directa con RAWG API para la obtención de datos de videojuegos en tiempo real.

## 🛠️ Tecnologías y Herramientas

* **Framework:** [React](https://reactjs.org/) + [Vite](https://vitejs.dev/)
* **Routing:** React Router DOM v6
* **Estilos:** CSS3 (Grid & Flexbox)
* **Contenedores:** Docker (Nginx para producción)
* **CI/CD:** GitHub Actions (Linter, Tests y Semantic Release)

## 💻 Instalación y Ejecución Local

Para poner en marcha el proyecto en tu entorno de desarrollo, sigue estos pasos:

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/JosephRangel/frontend2-week6-activity.git](https://github.com/JosephRangel/frontend2-week6-activity.git)
    cd frontend2-week6-activity
    ```

2.  **Instalar las dependencias:**
    ```bash
    npm install
    ```

3.  **Iniciar el servidor de desarrollo:**
    ```bash
    npm run dev
    ```
    La aplicación se ejecutará por defecto en `http://localhost:5173`.

## 🐳 Ejecución con Docker

El proyecto incluye un `Dockerfile` optimizado para producción. Para ejecutar la imagen sin necesidad de configurar el entorno de Node.js:

1.  **Construir la imagen:**
    ```bash
    docker build -t gamepedia-app .
    ```

2.  **Correr el contenedor:**
    ```bash
    docker run -d -p 8080:80 --name gamepedia-container gamepedia-app
    ```
    Accede a la aplicación desde tu navegador en `http://localhost:8080`.

## ⚙️ Automatización (CI/CD)

Este repositorio cuenta con flujos de trabajo automatizados mediante **GitHub Actions**:

* **Calidad de Código:** Validación automática de reglas de ESLint y ejecución de pruebas unitarias en cada Pull Request.
* **Versionado Semántico:** Uso de bots para la generación automática de versiones (`tags`) y actualización del historial de cambios (`CHANGELOG.md`) tras cada integración exitosa en la rama principal.

---
**Profesor:** Jose Antonio Rangel Reyes  
**Institución:** Cesun Universidad  
**Materia:** Desarrollo Frontend II