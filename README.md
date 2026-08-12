# spring-boot
Proyecto de Spring Boot

# SNPP API - Sistema de Gestión de Créditos Financieros

API RESTful desarrollada para la gestión integral de clientes, créditos, contratos, pagos y productos financieros.

---

## 🚀 Características Principales

- **Gestión de Clientes**: Registro, consulta, actualización y eliminación de clientes.
- **Gestión de Créditos**: Administración y seguimiento de créditos otorgados.
- **Gestión de Contratos**: Control de contratos vinculados a los créditos.
- **Gestión de Pagos**: Registro y seguimiento de los pagos realizados.
- **Gestión de Productos**: Catálogo de productos financieros disponibles.
- **Documentación Interactiva**: Integración con Swagger UI / OpenAPI 3.0.

---

## 🛠️ Tecnologías Utilizadas

- **Lenguaje / Framework**: Java / Spring Boot *(o el framework utilizado)*
- **Documentación de API**: OpenAPI v3 (Swagger UI)
- **Servidor Local**: `http://localhost:8081/snpp`

---

## 📚 Documentación de Endpoints

### 👥 Clientes (`/api/clientes`)

| Método | Endpoint | Descripción |
| :--- | :--- | :--- |
| `GET` | `/api/clientes` | Listar todos los clientes |
| `POST` | `/api/clientes` | Registrar un nuevo cliente |
| `GET` | `/api/clientes/{id}` | Buscar un cliente por ID |
| `PUT` | `/api/clientes/{id}` | Actualizar datos de un cliente |
| `DELETE` | `/api/clientes/{id}` | Eliminar un cliente |

---

### 💳 Créditos (`/api/creditos`)

| Método | Endpoint | Descripción |
| :--- | :--- | :--- |
| `GET` | `/api/creditos` | Listar todos los créditos |
| `POST` | `/api/creditos` | Registrar un nuevo crédito |
| `GET` | `/api/creditos/{id}` | Buscar un crédito por ID |
| `DELETE` | `/api/creditos/{id}` | Eliminar un crédito |

---

### 📄 Contratos (`/api/contratos`)

| Método | Endpoint | Descripción |
| :--- | :--- | :--- |
| `GET` | `/api/contratos` | Listar todos los contratos |
| `POST` | `/api/contratos` | Registrar un nuevo contrato |
| `GET` | `/api/contratos/{id}` | Buscar un contrato por ID |
| `DELETE` | `/api/contratos/{id}` | Eliminar un contrato |

---

### 💵 Pagos (`/api/pagos`)

| Método | Endpoint | Descripción |
| :--- | :--- | :--- |
| `GET` | `/api/pagos` | Listar todos los pagos |
| `POST` | `/api/pagos` | Registrar un nuevo pago |
| `GET` | `/api/pagos/{id}` | Buscar un pago por ID |
| `DELETE` | `/api/pagos/{id}` | Eliminar un pago |

#### Ejemplo de Cuerpo de Petición (POST `/api/pagos`)
```json
{
  "monto": 1000,
  "fecha": "2026-08-12",
  "idCliente": 1,
  "idCredito": 10
}