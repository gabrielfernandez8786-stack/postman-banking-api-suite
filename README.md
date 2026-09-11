# 🏦 Postman Banking API - Test Suite

Suite de pruebas automatizadas para una API de Banca Minorista, desarrollada con **Postman** y enfocada en la validación de flujos críticos: gestión de clientes, cuentas, transferencias, compliance y casos negativos.

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Tests-244%20Total-brightgreen?style=for-the-badge)

---

## 📋 Descripción

Este repositorio contiene una suite completa de pruebas de API que cubre:

- ✅ **Happy Path:** Creación de clientes, cuentas y transferencias exitosas.
- 🛡️ **Compliance:** Validación de límites diarios, cuentas congeladas y detección de fraudes (AML).
- ⚠️ **Casos Negativos:** Manejo de errores (campos faltantes, duplicados, saldos insuficientes).
- 🔄 **Flujos E2E:** Pruebas de extremo a extremo con preparación de datos.
- 🔒 **Idempotencia:** Prevención de transferencias duplicadas.

---

## 📂 Estructura del Proyecto
📦 postman-banking-api-suite
┣ 📂 postman
┃ ┣ 📜 Retail-Banking-API.postman_collection.json
┃ ┗ 📜 Banking-UAT.postman_environment.json
┣ 📂 docs
┃ ┗ 📂 images
┃ ┗ 📸 runner-results.png
┣ 📄 .gitignore
┗ 📄 README.md

---

## 🛠️ Tecnologías Utilizadas

- **Postman:** Ejecución de requests y scripts de validación.
- **JavaScript (ES6):** Scripts de Pre-request y Post-response.
- **Newman (opcional):** Ejecución de la suite desde línea de comandos.

---

## 🔄 Flujo de Pruebas

La suite está organizada en 8 carpetas que representan el flujo completo de un sistema bancario:

| # | Carpeta | Descripción |
|---|---------|-------------|
| 00 | `00_Environment & Setup` | Inicialización de reglas y datos base. |
| 01 | `01_Customer Management` | Creación y validación de clientes. |
| 02 | `02_Account Management` | Creación, validación y congelamiento de cuentas. |
| 03 | `03_Transaction Processing` | Depósitos y retiros. |
| 04 | `04_Funds Transfer & Payments` | Transferencias con idempotencia. |
| 05 | `05_Compliance & Validation` | Reglas AML, límites y fraudes. |
| 06 | `06_Negative Testing` | Casos de error y validaciones. |
| 07 | `07_Edge Cases & Risk Scenarios` | Escenarios extremos. |
| 08 | `08_End-to-End Business Flows` | Flujos completos E2E. |

---

## 📊 Resultados

Ejecución completa de la suite con el **Collection Runner**:

![Runner Results](docs/images/runner-results.png)

- ✅ **Tests Totales:** 244
- ✅ **Pasados:** 235
- ❌ **Fallidos (esperados):** 9 (Tests negativos)
- ⚠️ **Errores (esperados):** 3 (Bloqueos de seguridad)

> **Nota:** Los tests "fallidos" y "errores" son **intencionales**. Validan que el sistema rechace correctamente operaciones sospechosas o inválidas.

---

## 🚀 Cómo Ejecutar

### Opción 1: Postman (Manual)

1. Clona este repositorio:
   ```bash
   git clone https://github.com/gabrielfernandez8786-stack/postman-banking-api-suite.git
