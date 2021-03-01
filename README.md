## ⭐ Design Patterns
DesignPatterns es una colección de proyectos que muestran como manejar los siguientes conceptos:

- Clean Arquitecture usando las siguientes tecnologias:
    - .NET Core 3.1
    - ASP .NET Core 3.1
    - Entity Framework Core 3.1
    - Angular 9
    - MediatR
    - AutoMapper
    - FluentValidation
    - NUnit, FluentAssertions, Moq & Respawn
- Identity Server
    - Code flow Autentication
    - API Resources
    - API Scopes
    - Identity Resources
    - Client configuration
    - Identity Framework and Role based Authorization
- OpenID Connector
    - Cliente asp.net core
    - Cliente Angular (o cualquier cliente Javascript)

Los proyectos son los siguientes:

1. **[DesignPatterns.IdentityServer](https://github.com/isaacOjeda/DesignPatterns.IdentityServer).** Solución que implementa Identity Server 4, lo principal se puede aprender en este [quickstart](https://identityserver4.readthedocs.io/en/latest/quickstarts/0_overview.html). Está configurada para tener 2 clientes. **Angular** y **WebApp**.
2. **[DesignPatterns.Api](https://github.com/isaacOjeda/DesignPatterns.Api).** REST API que está protegida por IdentityServer. Sigue todos los principios de Clean Architecture siendo usada la plantilla de [Jason Taylor](https://jasontaylor.dev/clean-architecture-getting-started/).
3. **[DesignPatterns.Angular](https://github.com/isaacOjeda/DesignPatterns.Angular).** Aplicación Angular hosteada en asp.net core. Por medio de OpenID en Javascript realiza los intercambios de autenticación con IdentityServer. Tiene un TODO List de ejemplo que API gestiona.
4. **[DesignPatterns.Web](https://github.com/isaacOjeda/DesignPatterns.Web).** Realiza lo mismo que Angular, pero por medio de una aplicación de Razor Pages. (En desarrollo aun...)

## 🏁 Getting Started
Para empezar con el proyecto es necesario clonar los 4 repositorios mencionados arriba y ejecutarlos individualmente con `dotnet run`. También pueden ejecutarse desde Visual Studio, pero es importante que no se haga con IIS Express (los puertos son importantes).

## 🌐 Puertos
|Project  | HTTP | HTTPS|
|---------|------|-------|
|Identity |50000 | 50001 |
|API      |50002 | 50003 |
|Angular  |50004 | 50005 |
|Web      |50006 | 50007 |