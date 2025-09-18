📚 Gestión de Estudiantes - Android App

Una aplicación Android  desarrollada en Kotlin con Jetpack Compose para la gestión integral de estudiantes, conectada a una API RESTful.
🚀 Características

    Interfaz: Diseñada completamente con Jetpack Compose y Material Design 3

    Operaciones CRUD completas: Crear, leer, actualizar y eliminar estudiantes

    Conexión API REST: Integración con backend mediante Retrofit

    Manejo de errores robusto: Gestión de errores de conexión y autenticación

    Animaciones fluidas: Pantalla de splash con animaciones elegantes

    Confirmaciones de acción: Diálogos de confirmación para operaciones críticas

🛠️ Tecnologías Utilizadas

    Kotlin: Lenguaje de programación principal

    Jetpack Compose: UI declarativa moderna

    Retrofit: Cliente HTTP para APIs REST

    MVVM: Arquitectura Model-View-ViewModel

    Coroutines: Programación asíncrona

    Material Design 3: Sistema de diseño moderno

📦 Estructura del Proyecto

src/main/java/com/ufg/estudiantes/
├── data/
│   ├── ApiCallHandler.kt    # Manejador de llamadas API con manejo de errores
│   ├── ApiService.kt        # Interface de servicios API con Retrofit
│   └── EstudiantesRepository.kt # Repositorio para operaciones de datos
└── ui/theme/
    ├── EstudiantesScreen.kt  # Pantalla principal con UI en Compose
    ├── EstudiantesViewModel.kt # ViewModel con lógica de negocio
    └── MainActivity.kt       # Actividad principal con animación de splash

🔌 Endpoints API

La aplicación consume los siguientes endpoints:

    GET /estudiantes/ - Obtener lista de estudiantes

    GET /estudiantes/{id} - Obtener estudiante por ID

    POST /estudiantes/ - Crear nuevo estudiante

    PUT /estudiantes/{id} - Actualizar estudiante existente

    DELETE /estudiantes/{id} - Eliminar estudiante específico

    DELETE /estudiantes/admin/delete-all - Eliminar todos los estudiantes

🎨 Interfaz de Usuario
Pantalla de Splash

    Animación de escala y fade-in del logo

    Texto con aparición escalonada

    Botón de acceso con transición suave

Pantalla Principal

    Lista de estudiantes con cards informativas

    Formulario para agregar/editar estudiantes

    Botones de acción flotantes contextuales

    Diálogos de confirmación para eliminación

    Snackbars para feedback de operaciones

⚙️ Configuración
Requisitos Previos

    Android Studio (versión reciente)

    SDK de Android API 24+

    Conexión a internet para consumo de API

Variables de Entorno

La aplicación requiere una API Key válida para autenticación. Los errores 401 indican problemas de autenticación.
🚦 Estados de la Aplicación

La UI maneja varios estados:

    Cargando: Indicador de progreso durante operaciones

    Éxito: Mensajes de confirmación de operaciones

    Error: Manejo de errores de conexión y autenticación

    Confirmación: Diálogos para acciones destructivas

📱 Funcionalidades

    ✅ Listar todos los estudiantes

    ✅ Agregar nuevos estudiantes

    ✅ Editar estudiantes existentes

    ✅ Eliminar estudiantes individuales

    ✅ Eliminar todos los estudiantes (función admin)

    ✅ Búsqueda y filtros (pendiente de implementar)

    ✅ Validación de campos de entrada

🔒 Manejo de Errores

La aplicación detecta y maneja:

    Errores de conexión (Timeout, DNS, etc.)

    Errores de autenticación (401 Unauthorized)

    Errores del servidor (500 Internal Error)

    Errores de validación de datos

    Errores inesperados con mensajes descriptivos


🎯 Próximas Mejoras en camino 

    Búsqueda y filtrado de estudiantes

    Paginación de resultados

    Sincronización offline

    Exportación de datos

    Temas claros/oscuros

    Internacionalización (i18n)

    Tests unitarios e instrumentados

📄 Licencia

Este proyecto es desarrollado para fines académicos como parte de una practica para la materia de dispositivos moviles.

Desarrollado por José Pablo - 2025
Tecnologías: Kotlin, Jetpack Compose, Retrofit, MVVM.
