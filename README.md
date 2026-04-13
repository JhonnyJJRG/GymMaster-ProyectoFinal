# 🏋️‍♂️ GymMaster - Sistema Integral de Gestión de Gimnasio
Proyecto final para el curso de **Desarrollo de Servicios Web**.

## 👥 Integrantes del Equipo
* [cite_start]**Rondón González Jhonny Jesús**[cite: 6].
* [cite_start]Suyon Lescano Pablo Martin[cite: 7].
* [cite_start]Pulache Arevalo Erick Omar[cite: 8].
* [cite_start]Alcala Arata Cindy Yannet[cite: 9].
* [cite_start]Godoy Palacios Antonio Joaquin[cite: 10].

## 🏗️ Ecosistema de Microservicios
[cite_start]La solución se ha diseñado bajo una arquitectura de microservicios utilizando **.NET Core**, **C#** y **SQL Server**[cite: 13, 14, 15]. A continuación, se detallan los accesos a cada componente:

| Microservicio | Responsabilidad | Enlace al Repositorio | Puerto |
| :--- | :--- | :--- | :--- |
| **🔐 MS-Auth** | Autenticación, JWT y Control de Roles | [Ver Código](https://github.com/JhonnyJJRG/ExamenFinalGym-Auth) | [cite_start]5092 [cite: 91] |
| **🏢 MS-Administracion** | Gestión de Socios, Entrenadores y Membresías | [Ver Código](https://github.com/JhonnyJJRG/GymAdministracion) | [cite_start]5221 [cite: 91] |
| **🏋️‍♂️ MS-Rutinas** | Catálogo de Ejercicios y Planes de Entrenamiento | [Ver Código](https://github.com/JhonnyJJRG/GymRutinas) | [cite_start]5223 [cite: 91] |
| **💳 MS-Pagos** | Transacciones de Membresía y Control de Asistencias | [Ver Código](https://github.com/JhonnyJJRG/GymPagos) | [cite_start]5224 [cite: 91] |

---

### 🚀 Cómo ejecutar el proyecto
1.  [cite_start]**Base de Datos:** Ejecutar el archivo `script-bdgym.sql` en SQL Server Management Studio[cite: 89].
2.  [cite_start]**Configuración:** Actualizar las `ConnectionStrings` y la `Jwt:Key` en los archivos `appsettings.json` de cada microservicio[cite: 90].
3.  [cite_start]**Ejecución:** Iniciar los servicios en orden: Auth -> Administración -> Rutinas -> Pagos/Asistencias[cite: 91].
