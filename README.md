# proyecto-reservas-canchas
# 🏟️ SportReserva - Sistema de Reservas de Canchas Deportivas

![SportReserva Banner](https://images.unsplash.com/photo-1540747913346-19e32dc3e97e?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80)

SportReserva es una aplicación web moderna para la reserva de canchas deportivas. Permite a los usuarios explorar diferentes canchas, filtrar por deporte y ubicación, realizar reservas y gestionar sus reservas existentes.

## 📋 Tabla de Contenidos

- [Características](#-características)
- [Tecnologías Utilizadas](#-tecnologías-utilizadas)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Instalación](#-instalación)
- [Uso](#-uso)
- [API REST](#-api-rest)
- [Capturas de Pantalla](#-capturas-de-pantalla)
- [Contribución](#-contribución)
- [Licencia](#-licencia)
- [Contacto](#-contacto)

## ✨ Características

### Para Usuarios
- **Explorar Canchas**: Visualiza todas las canchas disponibles con imágenes y detalles
- **Filtros Avanzados**: Filtra canchas por:
  - Tipo de deporte (fútbol, tenis, pádel, baloncesto)
  - Ciudad (Madrid, Barcelona, Valencia)
  - Fecha disponible
- **Sistema de Reservas**: 
  - Selecciona fecha y hora
  - Elige duración (1-3 horas)
  - Calculo automático del precio total
  - Validación de datos en tiempo real
- **Gestión de Reservas**:
  - Visualiza todas tus reservas
  - Cancela reservas existentes
  - Persistencia de datos con localStorage

### Características Técnicas
- Diseño totalmente responsive
- Interfaz moderna y amigable
- Validación de formularios
- Formato automático de teléfono (xxx-xxx-xxxx)
- Almacenamiento local de datos
- Modal de reserva intuitivo

## 🛠 Tecnologías Utilizadas

### Frontend
- **HTML5** - Estructura semántica
- **CSS3** - Estilos personalizados y animaciones
- **JavaScript (ES6+)** - Lógica de negocio y manipulación del DOM
- **Bootstrap 5** - Framework CSS para diseño responsive
- **Font Awesome 6** - Iconos profesionales

### Herramientas de Desarrollo
- **Visual Studio Code** - Editor de código
- **Live Server** - Servidor de desarrollo local
- **Git** - Control de versiones

  <img width="354" height="368" alt="image" src="https://github.com/user-attachments/assets/e82293cd-132f-4fad-acf7-e0d6d283ce1b" />

  
## 🚀 Instalación

### Requisitos Previos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Visual Studio Code (recomendado)
- Git (opcional)

### Pasos de Instalación

1. **Clona el repositorio**
```bash
git clone https://github.com/tu-usuario/sportreserva.git

cd sportreserva

code .

Ejecuta con Live Server

Instala la extensión "Live Server" en VS Code

Haz clic derecho en index.html

Selecciona "Open with Live Server"

O simplemente abre el archivo index.html directamente en tu navegador.

💻 Uso
Realizar una Reserva
Explora las canchas disponibles en la página principal

Usa los filtros para encontrar la cancha ideal

Haz clic en "Reservar" en la tarjeta de la cancha deseada

Completa el formulario:

Fecha y hora

Duración

Datos personales

Teléfono (formato automático)

Confirma la reserva

Verás tu reserva en la sección "Mis Reservas"

Gestionar Reservas
Ve a la sección "Mis Reservas" en el menú

Visualiza todas tus reservas confirmadas

Usa el botón "Cancelar Reserva" si es necesario

Formato de Teléfono
El sistema acepta teléfonos con formato: 229-133-9124 (10 dígitos)

Se formatea automáticamente mientras escribes

Validación incluida

📡 API REST
Actualmente, el proyecto utiliza localStorage para la persistencia de datos. La estructura de datos simulada incluye:

Endpoints Simulados
GET /api/canchas

{
  id: 1,
  nombre: "Cancha de Fútbol 7",
  deporte: "futbol",
  ciudad: "madrid",
  ubicacion: "Madrid Centro",
  precio: 50,
  imagen: "url_imagen",
  descripcion: "Descripción de la cancha",
  horario: "9:00 - 22:00"
}

POST /api/reservas

{
  id: 123456789,
  canchaId: 1,
  canchaNombre: "Cancha de Fútbol 7",
  fecha: "2024-01-20",
  horaInicio: "18:00",
  duracion: 2,
  nombre: "Juan Pérez",
  telefono: "229-133-9124",
  email: "juan@email.com",
  precioTotal: 100


## 📁 Estructura del Proyecto
