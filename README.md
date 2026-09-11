# 🏦 Postman Banking API - Test Suite

Suite de pruebas automatizadas para una API de Banca Minorista, desarrollada con **Postman** y enfocada en la validación de flujos críticos: gestión de clientes, cuentas, transferencias, compliance y casos negativos.

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Tests-244%20Total-brightgreen?style=for-the-badge)
![Runner Results](docs/images/runner-results.png)

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
