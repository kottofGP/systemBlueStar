# Arquitectura de systemBlueStar

## Objetivo

SystemBlueStar es una plataforma de rastreo GPS desarrollada en C++,
orientada a la gestión de flotas, seguimiento de vehículos y recepción
de datos desde dispositivos GPS.

## Componentes principales

### Servidor GPS

Responsable de:

- Escuchar conexiones TCP.
- Recibir paquetes de dispositivos GPS.
- Identificar protocolos.
- Procesar información.
- Guardar datos en la base de datos.

### Base de Datos

Responsable de:

- Almacenar vehículos.
- Almacenar ubicaciones.
- Guardar eventos.
- Guardar usuarios.

### API

Responsable de:

- Entregar información al frontend.
- Consultar ubicaciones.
- Consultar historial.
- Gestionar usuarios.

### Frontend

Responsable de:

- Mostrar mapas.
- Mostrar vehículos.
- Mostrar historial.
- Administrar geocercas.

## Flujo de datos

GPS
↓
Servidor TCP
↓
Procesador de protocolos
↓
Base de datos
↓
API
↓
Frontend

## Tecnologías previstas

- C++
- SQLite
- HTTP
- TCP/IP
- Leaflet
- HTML
- CSS
- JavaScript

## Estructura general

systemBlueStar

├── servidor/
├── api/
├── frontend/
├── docs/
├── protocolos/
└── scripts/
