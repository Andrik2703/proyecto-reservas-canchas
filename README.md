# proyecto-reservas-canchas
<img width="645" height="966" alt="image" src="https://github.com/user-attachments/assets/a18e360a-13c9-4ad3-97b5-128b4b4facb2" />
<img width="623" height="527" alt="image" src="https://github.com/user-attachments/assets/061d06c5-ca44-4123-86e0-2537d5270faf" />

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
precio total: 100"


___________________________________________________________________________________________________________________________

# 🏟️ SportReserva - Sistema de Reservas de Canchas Deportivas

![Version](https://img.shields.io/badge/version-2.0.0-brightgreen)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?logo=fastapi)
![Python](https://img.shields.io/badge/Python-3.11+-blue)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3)

## 📋 Descripción General

SportReserva es una plataforma completa para la reserva de canchas deportivas que combina un frontend interactivo con una API REST profesional. Los usuarios pueden explorar canchas, filtrar por deporte y ciudad, realizar reservas y gestionar sus reservas existentes.

### ✨ Características Principales

- **Frontend**: Interfaz responsive con Bootstrap 5 y JavaScript vanilla
- **Backend**: API REST con FastAPI y PostgreSQL/SQLite
- **Autenticación**: JWT con soporte para roles (admin/cliente)
- **Persistencia dual**: LocalStorage + Base de datos
- **Modo offline**: Funciona sin conexión a internet
- **Documentación automática**: Swagger UI y ReDoc
- **Validaciones**: Pydantic para schemas, constraints en BD

## 🚀 Tecnologías Utilizadas

### Frontend
| Tecnología | Versión | Uso |
|------------|---------|-----|
| HTML5 | - | Estructura |
| CSS3 | - | Estilos personalizados |
| Bootstrap | 5.3.0 | Framework CSS |
| Font Awesome | 6.4.0 | Iconos |
| JavaScript | ES6 | Lógica de cliente |

### Backend
| Tecnología | Versión | Uso |
|------------|---------|-----|
| FastAPI | 0.104.1 | Framework web |
| SQLAlchemy | 2.0.23 | ORM |
| Pydantic | 2.5.0 | Validación |
| JWT | - | Autenticación |
| Alembic | 1.12.1 | Migraciones |
| PostgreSQL | - | Base de datos |

## 📦 Estructura del Proyecto
PROYECTO-RESERVAS-CANCHAS/
├── frontend/ # Aplicación web cliente
├── backend/ # API REST
├── docs/ # Documentación técnica
└── .vscode/ # Configuración IDE


## 🔧 Instalación y Configuración

### Requisitos Previos
- Python 3.11 o superior
- Node.js (opcional, para live server)
- Git

### Paso 1: Clonar el Repositorio
```bash
git clone https://github.com/tuusuario/PROYECTO-RESERVAS-CANCHAS.git
cd PROYECTO-RESERVAS-CANCHAS

Paso 2: Configurar Backend
<img width="328" height="520" alt="image" src="https://github.com/user-attachments/assets/35e5d370-4441-46dc-8353-e2e5b27008f8" />

Paso 3: Configurar Frontend
<img width="359" height="230" alt="image" src="https://github.com/user-attachments/assets/c63c64da-eb1e-4852-b5fa-3a68e1eaab22" />

Usuarios de Prueba
Administrador

Email: admin@sportreserva.com
Password: admin123
Rol: Administrador

Cliente Regular

Email: cliente@test.com
Password: cliente123
Rol: Cliente

Modelo de Datos
Entidades Principales
Usuario - Clientes y administradores

Deporte - Catálogo de deportes (fútbol, tenis, etc.)

Cancha - Instalaciones deportivas

Reserva - Reservas de canchas

Pago - Transacciones asociadas

Relaciones
Usuario 1:N Reserva

Cancha 1:N Reserva

Deporte 1:N Cancha

Reserva 1:1 Pago

🔒 Reglas de Negocio
✅ No se permiten reservas en fechas pasadas

✅ No hay solapamiento de horarios en misma cancha

✅ Email único por usuario

✅ Solo el propietario puede cancelar su reserva

✅ Horarios dentro del rango de operación

✅ Precio total automático (precio_hora × duración)

✅ Estados de reserva: pendiente → confirmada → completada/cancelada
