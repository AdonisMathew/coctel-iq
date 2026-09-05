# Setup local (Sprint 0 → Sprint 1)

Estos son los pasos para inicializar el proyecto en tu máquina una vez que descargues esta estructura base.

## 1. Inicializar Git

```bash
cd coctel-iq
git init
git add .
git commit -m "chore: estructura inicial del proyecto y documentación (Sprint 0)"
```

Creá el repo en GitHub (vacío, sin README) y conectalo:

```bash
git remote add origin https://github.com/AdonisMathew/coctel-iq.git
git branch -M main
git push -u origin main
```

## 2. Crear el proyecto ASP.NET Core

Requisitos: [.NET 8 SDK](https://dotnet.microsoft.com/download) instalado.

```bash
cd backend
dotnet new webapi -n CoctelIQ.Api -controllers
```

El flag `-controllers` usa controladores tradicionales (más fácil de entender al principio) en vez de Minimal APIs. Podemos migrar a Minimal APIs más adelante si querés practicar ese enfoque también.

## 3. Paquetes NuGet que vamos a necesitar (Sprint 1)

```bash
cd CoctelIQ.Api
dotnet add package Microsoft.EntityFrameworkCore.Design
dotnet add package Npgsql.EntityFrameworkCore.PostgreSQL
dotnet add package Microsoft.AspNetCore.Authentication.JwtBearer
dotnet add package Swashbuckle.AspNetCore
```

## 4. Verificar que corre

```bash
dotnet run
```

Deberías ver la API arrancar y poder abrir Swagger en `https://localhost:XXXX/swagger`.

## 5. Confirmar rama de trabajo (Git Flow simplificado)

Vamos a trabajar con:

- `main` → siempre estable, deployable
- `develop` → integración de features
- `feature/nombre-feature` → una rama por feature, mergeada a `develop` vía Pull Request

```bash
git checkout -b develop
git push -u origin develop
```

Cuando arranquemos el Sprint 1 (Usuarios + Auth), creamos `feature/auth-usuarios` desde `develop`.

---

**Avisame cuando tengas esto corriendo localmente y seguimos con el Sprint 1: el modelo de Usuario, el DbContext y la configuración de PostgreSQL.**
