
# 🏋️‍♂️ GymMaster - Sistema Integral de Gestión de Gimnasio
Proyecto final para el curso de **Desarrollo de Servicios Web**.

## 👥 Integrantes del Equipo
* **Rondón González Jhonny Jesús**
* Suyon Lescano Pablo Martin
* Pulache Arevalo Erick Omar
* Alcala Arata Cindy Yannet
* Godoy Palacios Antonio Joaquin

## 🏗️ Ecosistema de Microservicios
La solución se ha diseñado bajo una arquitectura de microservicios utilizando **.NET Core**, **C#** y **SQL Server**. A continuación, se detallan los accesos a cada componente:

| Microservicio | Responsabilidad | Enlace al Repositorio | Puerto |
| **🔐 MS-Auth** | Autenticación, JWT y Control de Roles | [Ver Código](https://github.com/JhonnyJJRG/ExamenFinalGym-Auth) | 5092 |
| **🏢 MS-Administracion** | Gestión de Socios, Entrenadores y Membresías | [Ver Código](https://github.com/JhonnyJJRG/GymAdministracion) | 5221 |
| **🏋️‍♂️ MS-Rutinas** | Catálogo de Ejercicios y Planes de Entrenamiento | [Ver Código](https://github.com/JhonnyJJRG/GymRutinas) | 5223 |
| **💳 MS-Pagos** | Transacciones de Membresía y Control de Asistencias | [Ver Código](https://github.com/JhonnyJJRG/GymPagos) | 5224 |

---

### 🚀 Cómo ejecutar el proyecto
1.  **Base de Datos:** Ejecutar el archivo `script-bdgym.sql` en SQL Server Management Studio para crear la estructura necesaria.
2.  **Configuración:** Actualizar las `ConnectionStrings` y la `Jwt:Key` en los archivos `appsettings.json` de cada microservicio para asegurar la conectividad y validación de tokens.
3.  **Ejecución:** Iniciar los servicios en el siguiente orden de dependencia: 
    * `Auth` -> `Administración` -> `Rutinas` -> `Pagos/Asistencias`.
