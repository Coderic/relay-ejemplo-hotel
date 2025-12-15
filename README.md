# 🏨 Hotel Booking - Reserva de Hoteles en Tiempo Real

Sistema de reserva de hoteles con disponibilidad en tiempo real construido con **Vue.js 3** y **[Relay Gateway](https://github.com/Coderic/Relay)**.

![Vue](https://img.shields.io/badge/Vue.js-3-4FC08D?logo=vue.js)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite)
![Relay](https://img.shields.io/badge/Relay-Gateway-blueviolet)

## 📖 Sobre este Ejemplo

**Hotel Booking** es un ejemplo funcional que demuestra cómo construir un sistema de reserva de hoteles con actualización de disponibilidad en tiempo real. Este ejemplo muestra:

- 🏨 **Búsqueda de hoteles** - Selección de destino, fechas y número de huéspedes
- 🛏️ **Selección de habitaciones** - Visualización de habitaciones disponibles
- ⚡ **Actualización en tiempo real** - La disponibilidad se sincroniza instantáneamente entre usuarios
- ⚠️ **Prevención de overbooking** - Múltiples usuarios no pueden reservar la misma habitación
- 📊 **Gestión de reservas** - Vista de todas las reservas activas

Este ejemplo pertenece a la colección de ejemplos de **[Relay Gateway](https://github.com/Coderic/Relay)**, un gateway de comunicación en tiempo real diseñado para ser inmutable y agnóstico.

## 🚀 Inicio Rápido

### Prerrequisitos

- Node.js 18+ o Docker
- Relay Gateway ejecutándose (ver [documentación de Relay](https://relay.coderic.net))

### Instalación

```bash
# Clonar el repositorio
git clone https://github.com/Coderic/hotel.git
cd hotel

# Instalar dependencias
npm install
```

### Configuración

Asegúrate de tener Relay Gateway ejecutándose. Puedes usar el endpoint público para pruebas:

```javascript
// En tu código, el conector se conecta a:
const relay = new RelayConector('http://demo.relay.coderic.net');
```

O ejecuta Relay localmente:

```bash
# Opción 1: Con npx (recomendado para pruebas)
npx @coderic/relay

# Opción 2: Con Docker Compose
docker compose up -d
```

### Desarrollo

```bash
# Iniciar servidor de desarrollo
npm run dev
```

Abre tu navegador en `http://localhost:5173` (o el puerto que Vite asigne).

### Producción

```bash
# Construir para producción
npm run build

# Los archivos estarán en la carpeta dist/
```

## 🎯 Uso

1. **Abrir múltiples pestañas** para simular diferentes usuarios
2. **Buscar hoteles** seleccionando destino, fechas y huéspedes
3. **Seleccionar habitaciones** - Observa cómo la disponibilidad se actualiza en tiempo real
4. **Realizar reservas** - Las habitaciones se bloquean automáticamente para otros usuarios
5. **Ver el dashboard** - Monitorea todas las reservas en tiempo real

## 🔗 Enlaces

- 📦 [Repositorio](https://github.com/Coderic/hotel)
- 🐛 [Issues](https://github.com/Coderic/hotel/issues)
- 🌐 [Demo en línea](https://coderic.org/hotel/)
- 📚 [Documentación de Relay](https://relay.coderic.net)
- ⚡ [Relay Gateway](https://github.com/Coderic/Relay)

## 🛠️ Tecnologías

- **Vue.js 3** - Framework JavaScript progresivo
- **Vite** - Build tool y dev server
- **Relay Gateway** - Gateway de comunicación en tiempo real
- **Socket.io** - Comunicación WebSocket

## 📝 Licencia

MIT
