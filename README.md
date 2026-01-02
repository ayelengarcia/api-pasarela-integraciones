# API Pasarela – Integración de Servicios Backend

Proyecto backend orientado a integraciones entre múltiples servicios internos y plataformas externas, desarrollado bajo un enfoque de arquitectura desacoplada y orientada a servicios.

---

## 🧩 Descripción del proyecto

Diseño e implementación de una **API Pasarela** utilizada como capa intermedia para conectar distintos **microservicios backend desplegados en máquinas virtuales independientes**, permitiendo la comunicación segura y controlada con plataformas externas.

La solución fue utilizada para integrar servicios internos con **scripts y flujos automatizados en Botmaker**, facilitando el intercambio de datos y la ejecución de procesos entre sistemas.

---

## 🏗 Arquitectura

- **Server API Sifaco**  
  Servicio backend desplegado en una VM interna, encargado de la lógica principal y exposición de endpoints privados para sistema de facturación automática.
  Repo: [https://github.com/ayelengarcia/server-api-sifaco](https://github.com/ayelengarcia/Server_api_sifaco)

- **Server BDC**  
  Servicio backend independiente, alojado en una segunda VM interna, responsable de operaciones específicas y procesamiento de datos de clientes.
  Repo: [https://github.com/ayelengarcia/Server_BDC](https://github.com/ayelengarcia/Server_BDC)

- **API Pasarela (Semi-abierta)**  
  Capa intermedia que centraliza:
  - Validación de requests
  - Normalización de datos
  - Exposición controlada de endpoints
  - Comunicación entre servicios internos y sistemas externos
  Repo: [https://github.com/ayelengarcia/Server_pasarela](https://github.com/ayelengarcia/Server_pasarela)

- **Integración externa**
  - Consumo mediante scripts personalizados en **Botmaker**
  - Webhooks y requests HTTP controlados
  Repo: [https://github.com/ayelengarcia/Scripts-botmaker-y-otros](https://github.com/ayelengarcia/Scripts-botmaker-y-otros)

---

## 🀄 Diagrama

<img width="750" height="649" alt="apipasarela" src="https://github.com/user-attachments/assets/c4433527-e0a7-4929-b5a8-daf79d7e8d95" />

---

## 🛠 Tecnologías utilizadas

- Node.js
- Express
- APIs REST
- Scripts de integración
- Arquitectura orientada a servicios
- Despliegue en máquinas virtuales (Azure)
- Integraciones con plataformas externas (Botmaker)

---

## 👩‍💻 Rol y responsabilidades

- Diseño de la arquitectura de integración
- Desarrollo backend end-to-end
- Implementación de APIs REST
- Integración con servicios externos mediante scripts
- Coordinación de flujos entre múltiples servidores
- Mantenimiento y evolución de la solución

---

## 📈 Impacto

- Desacople entre servicios internos
- Integraciones más seguras y escalables
- Reducción de dependencias directas entre sistemas
- Facilitó la automatización de procesos mediante bots
