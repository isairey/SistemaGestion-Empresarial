# 🧾 DjangoSIGE — Sistema Integrado de Gestión Empresarial

[![Build Status](https://travis-ci.org/thiagopena/djangoSIGE.svg?branch=master)](https://travis-ci.org/thiagopena/djangoSIGE)

**DjangoSIGE** es un sistema ERP (Enterprise Resource Planning) desarrollado con **Django (Python)**, diseñado para gestionar procesos empresariales como inventario, ventas, finanzas y facturación electrónica.

---

## 🚀 Características principales

- 📦 Gestión de productos, clientes, proveedores y empresas  
- 🔐 Sistema de autenticación (login/logout)  
- 👤 Roles y permisos por usuario  
- 🧾 Generación de presupuestos y órdenes de compra/venta en PDF  
- 📊 Módulo financiero:
  - Plan de cuentas  
  - Flujo de caja  
  - Registro de movimientos  
- 📦 Control de inventario  
- 🧮 Módulo fiscal:
  - Generación y almacenamiento de facturas  
  - Validación de XML (NF-e / NFC-e)  
  - Emisión y cancelación de comprobantes  
  - Integración con SEFAZ *(entorno de pruebas)*  
- 🌐 Interfaz intuitiva y en idioma portugués  

---

## 🧱 Tecnologías utilizadas

- **Python 3**
- **Django 3.1.7**
- **HTML / CSS / JavaScript**
- **jQuery & DataTables**
- **Bootstrap / Material Design**

---

## 📦 Dependencias

- Python >= 3.5  
- Django == 3.1.7  
- geraldo (generación de PDFs)  
- PySIGNFe *(opcional para facturación electrónica)*  
- Apache2 + mod_wsgi *(opcional para producción)*  

---

## ⚙️ Instalación

### 1️⃣ Instalar dependencias del sistema (Linux)

```bash
sudo apt update
sudo apt install -y libxml2 gcc python3-dev libxml2-dev libxslt1-dev zlib1g-dev python3-pip
```

### 2️⃣ Instalar dependencias del proyecto
```
pip install -r requirements.txt
```
### 3️⃣ Configuración del sistema

Editar archivo:
```
djangosige/configs/configs.py
```
### 4️⃣ Generar variables de entorno
```
python contrib/env_gen.py
```

### 5️⃣ Migraciones
```
python manage.py migrate
```
### 6️⃣ Crear usuario administrador
```
python manage.py createsuperuser
```
### 7️⃣ Ejecutar servidor
```
python manage.py runserver
```

Abrir en navegador:
```
👉 http://localhost:8000
```
---

## 🌐 Estado del proyecto

- 🚧 Proyecto en desarrollo activo
- ⚠️ Algunas funciones fiscales requieren configuración adicional

### 🛠️ Despliegue (Producción)

Opcionalmente puedes usar:
```
Apache2
mod_wsgi
```
---

## 🤝 Contribuciones

Las contribuciones son bienvenidas:

- Fork del repositorio
- Crear una rama (feature/nueva-funcionalidad)
- Realizar cambios
- Enviar Pull Request

---

## 🧩 Créditos

- AdminBSB Material Design
- Geraldo
- jQuery Mask Plugin
- DataTables
- jQuery Multiselect


## 📩 Soporte

🐛 Issues: https://github.com/isairey/SistemaGestion-Empresarial/issues
📧 Email: isaireyes2003@gmail.com

---

## 👨‍💻 Autor

**Isai Reyes**

---

## 📄 Licencia

License MIT.
