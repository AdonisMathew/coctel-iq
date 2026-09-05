# 🍸 CoctelIQ

> Una plataforma estilo Duolingo para aprender bartending: cócteles, técnicas y teoría de coctelería, con lecciones, quizzes y gamificación.

![Status](https://img.shields.io/badge/status-en%20desarrollo-yellow)
![.NET](https://img.shields.io/badge/.NET-8-512BD4)
![License](https://img.shields.io/badge/license-MIT-blue)

## 📖 Sobre el proyecto

CoctelIQ nace de combinar dos mundos: bartending profesional y desarrollo de software. La idea es aprender (y enseñar) coctelería de forma gamificada — lecciones cortas, quizzes, recetas, y un sistema de progreso que premia la constancia (rachas, XP, niveles, ranking).

Es también un proyecto de portfolio: documentado, versionado y desarrollado siguiendo buenas prácticas de ingeniería de software (arquitectura en capas, control de versiones con Git Flow, testing, CI/CD).

## ✨ Features (MVP)

- [ ] **Autenticación de usuarios** (registro, login, JWT)
- [ ] **Lecciones y módulos** organizados por categoría (espirituosos, técnicas, historia, mixología)
- [ ] **Quizzes interactivos** con corrección automática
- [ ] **Catálogo de recetas** de cócteles con ingredientes, pasos y dificultad
- [ ] **Sistema de progreso**: XP, niveles, lecciones completadas
- [ ] **Rachas** (streaks) de días consecutivos estudiando
- [ ] **Ranking social** (leaderboard) entre usuarios

## 🏗️ Stack tecnológico

| Capa | Tecnología |
|---|---|
| Backend | ASP.NET Core 8 Web API (C#) |
| ORM | Entity Framework Core |
| Base de datos | PostgreSQL |
| Autenticación | JWT + ASP.NET Identity |
| Frontend | *(a definir)* |
| Testing | xUnit |
| Documentación API | Swagger / OpenAPI |
| Control de versiones | Git (Git Flow) |

## 📂 Estructura del repositorio

```
coctel-iq/
├── backend/          # API en ASP.NET Core
├── frontend/         # Cliente web
├── docs/             # Documentación técnica (arquitectura, DB, decisiones)
│   └── database-design.md
└── README.md
```

## 🗺️ Roadmap

| Sprint | Objetivo | Estado |
|---|---|---|
| 0 | Setup del repo, documentación, diseño de base de datos | 🟡 En curso |
| 1 | API base: Usuarios + Autenticación (JWT) | ⬜ Pendiente |
| 2 | Lecciones + Preguntas + lógica de quiz | ⬜ Pendiente |
| 3 | Catálogo de Cócteles/Recetas | ⬜ Pendiente |
| 4 | Progreso de usuario, XP y niveles | ⬜ Pendiente |
| 5 | Rachas + Ranking social | ⬜ Pendiente |
| 6 | Frontend conectado al backend | ⬜ Pendiente |
| 7 | Testing, pulido y deploy | ⬜ Pendiente |

## 🚀 Cómo correr el proyecto

*(Se completa en el Sprint 1, cuando exista código funcional)*

## 🧠 Decisiones de diseño

Las decisiones técnicas importantes (por qué PostgreSQL y no SQL Server, por qué esta estructura de carpetas, etc.) se documentan en [`docs/`](./docs) a medida que se toman.

## 👤 Autor

Proyecto desarrollado por AdonisMathew como parte de su portfolio, combinando experiencia como bartender profesional con formación en desarrollo de software.

## 📄 Licencia

MIT — libre para usar, modificar y aprender de este código.
