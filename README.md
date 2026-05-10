# 🚀 Software FJ - Sistema Integral de Gestión de Servicios y Reservas

Sistema desarrollado en Python orientado a la gestión de clientes, servicios y reservas para la empresa **Software FJ**.  
El proyecto implementa principios fundamentales de **Programación Orientada a Objetos (POO)**, manejo avanzado de excepciones y arquitectura modular.

---

# 📌 Características Principales

✅ Gestión de clientes  
✅ Gestión de servicios  
✅ Creación y confirmación de reservas  
✅ Cancelación de reservas  
✅ Manejo de excepciones personalizadas  
✅ Registro de errores en archivos logs  
✅ Arquitectura modular  
✅ Programación Orientada a Objetos (POO)  
✅ Encapsulación  
✅ Herencia  
✅ Polimorfismo  
✅ Abstracción  
✅ Sobrescritura de métodos  
✅ Validaciones robustas  

---

# 🏗️ Arquitectura del Proyecto

```text
Software-FJ/
│
├── cliente.py
├── servicio.py
├── servicios_especificos.py
├── reserva.py
├── excepciones.py
├── main.py
├── logs.txt
└── README.md
```

---

# 📂 Descripción de los Módulos

## 🔹 cliente.py
Gestiona toda la información relacionada con los clientes.

### Funcionalidades:
- Validación de nombres
- Validación de correos electrónicos
- Validación de teléfonos
- Validación de identificación
- Actualización de datos
- Encapsulación de atributos

---

## 🔹 servicio.py
Clase abstracta base para todos los servicios del sistema.

### Implementa:
- Abstracción
- Métodos abstractos
- Validaciones generales
- Verificación de disponibilidad
- Manejo de errores

---

## 🔹 servicios_especificos.py
Contiene los servicios especializados que heredan de `Servicio`.

### Clases implementadas:
- `ReservaSala`
- `AlquilerEquipo`
- `Asesoria`

### Conceptos aplicados:
- Herencia
- Polimorfismo
- Sobrescritura de métodos

---

## 🔹 reserva.py
Gestiona el proceso de reservas dentro del sistema.

### Funcionalidades:
- Confirmación de reservas
- Cancelación de reservas
- Validación de disponibilidad
- Control de estados
- Manejo avanzado de excepciones

---

## 🔹 excepciones.py
Centraliza todas las excepciones personalizadas y el sistema de logs.

### Excepciones:
- `SoftwareFJError`
- `ClienteError`
- `ReservaError`
- `DisponibilidadError`

### Sistema de logs:
Los errores se almacenan automáticamente en:

```text
logs.txt
```

---

## 🔹 main.py
Archivo principal encargado de ejecutar el sistema completo.

### Incluye:
- Creación de clientes
- Creación de servicios
- Creación de reservas
- Confirmaciones
- Cancelaciones
- Pruebas de errores controlados

---

# 🧠 Conceptos de Programación Aplicados

## 🔒 Encapsulación
Uso de atributos privados y protegidos:

```python
self.__nombre
self._precio_base
```

---

## 🧬 Herencia
Las clases específicas heredan de una clase base:

```python
class ReservaSala(Servicio)
```

---

## 🔁 Polimorfismo
Cada servicio redefine sus propios métodos:

```python
calcular_costo()
descripcion()
```

---

## 🧩 Abstracción
Uso de clases abstractas:

```python
class Servicio(ABC)
```

---

## ⚠️ Manejo de Excepciones
Implementación de:
- `try`
- `except`
- `else`
- `finally`

y excepciones personalizadas.

---

# 🛡️ Sistema de Logs

Todos los errores importantes quedan registrados automáticamente en:

```text
logs.txt
```

### Ejemplo:

```text
[2026-05-08 00:31:52] | TIPO: DisponibilidadError | CONTEXTO: Reserva.confirmar_reserva | DETALLE: Fallo de disponibilidad...
```

---

# ▶️ Cómo Ejecutar el Proyecto

## 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/USUARIO/REPOSITORIO.git
```

---

## 2️⃣ Entrar a la carpeta

```bash
cd Software-FJ
```

---

## 3️⃣ Ejecutar el sistema

```bash
python main.py
```

---

# 🖥️ Requisitos

- Python 3.10 o superior
- Visual Studio Code (opcional)
- Git (opcional)

---

# 📋 Ejemplos de Funcionalidades

## ✔️ Crear Cliente

```python
cliente = Cliente(
    "Andrés López",
    "andres@gmail.com",
    "3201234567",
    "123456789"
)
```

---

## ✔️ Crear Servicio

```python
sala = ReservaSala(
    "Sala Ejecutiva",
    80000,
    15
)
```

---

## ✔️ Crear Reserva

```python
reserva = Reserva(
    cliente,
    sala,
    3
)
```

---

# 📊 Estado del Proyecto

✅ Proyecto funcional  
✅ Arquitectura modular completa  
✅ Validaciones implementadas  
✅ Manejo de errores implementado  
✅ Sistema de logs funcionando  

---

# 👨‍💻 Autores

## ANDRES FELIPE LOPEZ ARENAS
## REAGON CROWELL RAMIREZ SANCHEZ
## OSCAR DAVID GARAY MORENO
## REAGON CROWELL RAMIREZ SANCHEZ

Proyecto académico desarrollado para aplicar conceptos avanzados de Programación Orientada a Objetos en Python.

---

# 📄 Licencia

Este proyecto fue desarrollado con fines académicos y educativos.