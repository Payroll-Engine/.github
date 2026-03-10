<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Payroll-Engine/PayrollEngine/blob/main/images/logo/NameInversShadow.png">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/Payroll-Engine/PayrollEngine/blob/main/images/logo/NameNormalShadow.png">
    <img alt="Payroll Engine" src="https://github.com/Payroll-Engine/PayrollEngine/blob/main/images/logo/NameNormalShadow.png" width="460px" />
  </picture>
</p>

<p align="center">
  <strong>The open-source payroll automation framework.</strong><br />
  Build multi-country, multi-industry payroll applications with configurable regulation layers.
</p>

<p align="center">
  <a href="https://github.com/Payroll-Engine/PayrollEngine/releases"><img alt="GitHub release" src="https://img.shields.io/github/v/release/Payroll-Engine/PayrollEngine?include_prereleases&logo=github" /></a>
  <a href="https://github.com/Payroll-Engine/PayrollEngine/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-green.svg" /></a>
  <a href="https://www.nuget.org/packages/PayrollEngine.Client.Services"><img alt="NuGet" src="https://img.shields.io/nuget/vpre/PayrollEngine.Client.Services?logo=nuget&color=blue" /></a>
  <a href="https://github.com/orgs/Payroll-Engine/packages"><img alt="Docker" src="https://img.shields.io/badge/ghcr.io-images-blue?logo=docker" /></a>
</p>

<p align="center">
  <a href="https://payrollengine.org/docs"><strong>Documentation</strong></a> ·
  <a href="https://payrollengine.org/docs/ContainerSetup"><strong>Quick Start</strong></a> ·
  <a href="https://github.com/Payroll-Engine/PayrollEngine/releases"><strong>Releases</strong></a> ·
  <a href="https://github.com/Payroll-Engine/PayrollEngine/discussions"><strong>Discussions</strong></a>
</p>

---

## What is the Payroll Engine?

The Payroll Engine is a framework for developing payroll applications. Payroll logic is **not hardcoded** — business rules are defined in configurable [regulation layers](https://payrollengine.org/docs/Regulations) that can be stacked, overridden, and shared between tenants. This makes the engine adaptable to any country, any industry, and any HR platform.

## Who Is This For?

| Role | Description | Interface |
|:---|:---|:---|
| **Provider** | Software vendors and payroll service providers who host and operate the engine | REST API |
| **Regulator** | Payroll domain experts who define country- or industry-specific calculation rules | No-Code · C# Scripting |
| **Automator** | DevOps and integration engineers who connect the engine to HR platforms and data pipelines | .NET Client SDK |

## Quick Start

The engine runs as a Docker container stack — Docker is the only prerequisite.

```sh
mkdir payroll-engine && cd payroll-engine
echo "DB_PASSWORD=PayrollStrongPass789" > .env
curl -O https://raw.githubusercontent.com/Payroll-Engine/PayrollEngine/main/docker-compose.yml
docker compose up -d
```

| Service | URL |
|:---|:---|
| Web Application | http://localhost:8081 |
| Backend API | http://localhost:5001 |

→ Full setup guide at [payrollengine.org/docs/ContainerSetup](https://payrollengine.org/docs/ContainerSetup)

## .NET Integration

```sh
dotnet add package PayrollEngine.Client.Services
```

→ See [Client Services](https://payrollengine.org/docs/ClientServices) for the full integration guide.

## Repositories

| Repository | Description | |
|:---|:---|:---|
| [PayrollEngine](https://github.com/Payroll-Engine/PayrollEngine) | Main repo — Docker stack, examples, tests | [![release](https://img.shields.io/github/v/release/Payroll-Engine/PayrollEngine?include_prereleases&label=&logo=github)](https://github.com/Payroll-Engine/PayrollEngine/releases) |
| [Backend](https://github.com/Payroll-Engine/PayrollEngine.Backend) | REST API server + SQL Server persistence | [![Docker](https://img.shields.io/badge/ghcr.io-image-blue?logo=docker)](https://github.com/orgs/Payroll-Engine/packages) |
| [WebApp](https://github.com/Payroll-Engine/PayrollEngine.WebApp) | Blazor web application | [![Docker](https://img.shields.io/badge/ghcr.io-image-blue?logo=docker)](https://github.com/orgs/Payroll-Engine/packages) |
| [PayrollConsole](https://github.com/Payroll-Engine/PayrollEngine.PayrollConsole) | CLI for automation, testing, data import | [![Docker](https://img.shields.io/badge/ghcr.io-image-blue?logo=docker)](https://github.com/orgs/Payroll-Engine/packages) |
| [Client.Services](https://github.com/Payroll-Engine/PayrollEngine.Client.Services) | .NET Client SDK (NuGet entry package) | [![NuGet](https://img.shields.io/nuget/vpre/PayrollEngine.Client.Services?label=&logo=nuget&color=blue)](https://www.nuget.org/packages/PayrollEngine.Client.Services) |
| [Client.Scripting](https://github.com/Payroll-Engine/PayrollEngine.Client.Scripting) | Scripting API for regulation development | [![NuGet](https://img.shields.io/nuget/vpre/PayrollEngine.Client.Scripting?label=&logo=nuget&color=blue)](https://www.nuget.org/packages/PayrollEngine.Client.Scripting) |
| [Client.Test](https://github.com/Payroll-Engine/PayrollEngine.Client.Test) | Test runner library | [![NuGet](https://img.shields.io/nuget/vpre/PayrollEngine.Client.Test?label=&logo=nuget&color=blue)](https://www.nuget.org/packages/PayrollEngine.Client.Test) |

→ Full repository map at [payrollengine.org/docs/Repositories](https://payrollengine.org/docs/Repositories)

## License

MIT — free for any use. All third-party dependencies use MIT or Apache 2.0 licenses.
