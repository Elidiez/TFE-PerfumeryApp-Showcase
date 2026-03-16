# TFE-PerfumeryApp-Showcase
# FormuLab - Advanced Perfumery Formulation System

![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-%237F52FF.svg?style=for-the-badge&logo=kotlin&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-%23039BE5.svg?style=for-the-badge&logo=firebase)

**FormuLab** is a native Android mobile application aimed at optimizing the workflow of independent perfumers and formulation students. The system automates dilution calculations, manages raw material databases, and allows for the structured design of olfactory formulas under high security standards.

> **Intellectual Property Notice:** This repository serves exclusively as a technical portfolio (Showcase). The original source code is proprietary and kept in a closed environment, as the software is currently in a pre-commercialization phase. I am fully available for architecture reviews and code demonstrations during recruitment processes or technical interviews.

---

## Core Features

* **Raw Material Management:** Local database engine for efficient querying of hundreds of ingredients, indexed by CAS number, olfactory family, and regulatory restrictions (IFRA).
* **Algorithmic Dilution Engine:** Precise calculation module for determining solute/solvent proportions when reducing concentrations.
* **Structured Composer:** Formula design tool based on the traditional olfactory pyramid (top, heart, and base notes) with automatic calculation of final concentrations (EDC, EDT, EDP).
* **Biometric Authentication:** BiometricPrompt API integration to restrict access to the private formulas section using device hardware (fingerprint/facial recognition).
* **Cryptography (E2EE):** Implementation of end-to-end encryption to guarantee the industrial secrecy of the formulas stored in the cloud.

## Architecture and Tech Stack

The project has been developed applying **Clean Architecture** principles and the **MVVM (Model-View-ViewModel)** design pattern recommended in official Android guidelines.

* **Native Development:** Kotlin (SDK 28+).
* **User Interface (UI):** Jetpack Compose (Declarative UI).
* **Data Persistence (Local):** Room (SQLite) implementing initial load deserialization with GSON.
* **Data Persistence (Cloud):** Cloud Firestore (NoSQL document-oriented database).
* **Identity Management:** Firebase Authentication integrated with Google Single Sign-On (SSO).
* **Concurrency and Asynchrony:** Kotlin Coroutines and reactive flows (StateFlow/Flow).

## Visual and Technical Documentation


![Diagrama de Base de Datos](umlLocal.png)
![Diagrama General App](AppDiagram.png)



## License and Copyright

**Copyright © 2026 Elida María Diez Gómez. All rights reserved.**

This repository, including its documentation, design schemas (UI/UX), data model, and described architecture, is not distributed under any open-source license. The reproduction, distribution, modification, copying, or commercial use of any element presented in this project without the express, prior, and written authorization of the author is strictly prohibited.
Showcase TFE: App Android nativa (Kotlin + Compose) para formulación en perfumería. Arquitectura MVVM, Room, Firebase y Seguridad Biométrica E2EE.

_____

# FormuLab - Sistema Avanzado de Formulación de Perfumería

![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-%237F52FF.svg?style=for-the-badge&logo=kotlin&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-%23039BE5.svg?style=for-the-badge&logo=firebase)

**FormuLab** es una aplicación móvil nativa para Android orientada a la optimización del flujo de trabajo de perfumistas independientes y estudiantes de formulación. El sistema automatiza el cálculo de diluciones, gestiona bases de datos de materias primas y permite el diseño estructurado de fórmulas olfativas bajo altos estándares de seguridad.

> **Aviso de Propiedad Intelectual:** El presente repositorio funciona exclusivamente como un portfolio técnico (Showcase). El código fuente original es de carácter privativo y se mantiene en un entorno cerrado, dado que el software se encuentra en fase de pre-comercialización. Estoy a disposición para realizar revisiones de arquitectura y demostraciones de código durante procesos de selección o entrevistas técnicas.

## Funcionalidades Principales

* **Gestión de Materias Primas:** Motor de base de datos local para la consulta eficiente de cientos de ingredientes, indexados por código CAS, familia olfativa y restricciones regulatorias (IFRA).
* **Motor Algorítmico de Diluciones:** Módulo de cálculo preciso para la determinación de proporciones soluto/solvente en la rebaja de concentraciones.
* **Compositor Estructurado:** Herramienta de diseño de fórmulas basada en la pirámide olfativa tradicional (notas de salida, corazón y fondo) con cálculo automático de concentraciones finales (EDC, EDT, EDP).
* **Autenticación Biométrica:** Integración de la API BiometricPrompt para restringir el acceso a la sección privada de fórmulas mediante hardware (huella dactilar/reconocimiento facial).
* **Criptografía (E2EE):** Implementación de cifrado de extremo a extremo para garantizar el secreto industrial de las fórmulas almacenadas en la nube.

## Arquitectura y Stack Tecnológico

El proyecto ha sido desarrollado aplicando los principios de **Clean Architecture** y el patrón de diseño **MVVM (Model-View-ViewModel)** recomendado en las directrices oficiales de Android.

* **Desarrollo Nativo:** Kotlin (SDK 28+).
* **Interfaz de Usuario (UI):** Jetpack Compose (UI Declarativa).
* **Persistencia de Datos (Local):** Room (SQLite) implementando deserialización de carga inicial con GSON.
* **Persistencia de Datos (Cloud):** Cloud Firestore (Base de datos NoSQL orientada a documentos).
* **Gestión de Identidad:** Firebase Authentication integrado con Google Single Sign-On (SSO).
* **Concurrencia y Asincronía:** Kotlin Coroutines y flujos reactivos (StateFlow/Flow).

## Documentación Técnica y Visual

![Diagrama de Base de Datos](umlLocal.png)
![Diagrama General App](AppDiagram.png)

## Licencia y Derechos de Autor

**Copyright © 2026 Elida María Diez Gómez. Todos los derechos reservados.**

Este repositorio, incluyendo su documentación, esquemas de diseño (UI/UX), modelo de datos y arquitectura descrita, no se distribuye bajo ninguna licencia de código abierto. Queda estrictamente prohibida la reproducción, distribución, modificación, copia o uso comercial de cualquier elemento expuesto en este proyecto sin la autorización expresa, previa y por escrito de la autora.
