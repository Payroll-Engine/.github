<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Payroll-Engine/PayrollEngine/blob/main/images/logo/NameInversShadow.png">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/Payroll-Engine/PayrollEngine/blob/main/images/logo/NameNormalShadow.png">
    <img alt="Payroll Engine" src="https://github.com/Payroll-Engine/PayrollEngine/blob/main/images/logo/NameNormalShadow.png" width="460px" />
  </picture>
</p>

<p align="center">
  <strong>The open-source payroll automation framework.</strong><br/>
  Build multi-country, multi-industry payroll applications with composable regulation layers.
</p>

<p align="center">
  <a href="https://github.com/Payroll-Engine/PayrollEngine/actions"><img alt="Build" src="https://img.shields.io/github/actions/workflow/status/Payroll-Engine/PayrollEngine/build.yml?logo=github" /></a>
  <a href="https://github.com/Payroll-Engine/PayrollEngine/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-green.svg" /></a>
  <a href="https://github.com/Payroll-Engine/PayrollEngine/releases"><img alt="Release" src="https://img.shields.io/github/v/release/Payroll-Engine/PayrollEngine?include_prereleases&logo=github" /></a>
  <a href="https://www.nuget.org/packages/PayrollEngine.Client.Services"><img alt="NuGet" src="https://img.shields.io/nuget/vpre/PayrollEngine.Client.Services?logo=nuget&color=blue" /></a>
  <a href="https://github.com/orgs/Payroll-Engine/packages"><img alt="Docker" src="https://img.shields.io/badge/ghcr.io-images-blue?logo=docker" /></a>
</p>

<p align="center">
  <a href="https://payrollengine.org"><strong>Website</strong></a>
  &nbsp;·&nbsp;
  <a href="https://payrollengine.org/GetStarted/Overview/"><strong>Get Started</strong></a>
  &nbsp;·&nbsp;
  <a href="https://payrollengine.org/GetStarted/ContainerSetup/"><strong>Quick Start</strong></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/Payroll-Engine/PayrollEngine/discussions"><strong>Discussions</strong></a>
</p>

---

## What is the Payroll Engine?

The Payroll Engine is a framework for building payroll applications. Payroll logic lives in **configurable regulation layers** — not hardcoded. Layers are stacked, overridden, and shared across tenants, countries, and industries.

Embed it via **REST API**, deploy it via **Docker**, or automate it with the **.NET Client SDK**.

## Three Roles

| Role | Who | Interface |
|:--|:--|:--|
| **Provider** | HR-tech platforms, EOR providers | REST API · OpenAPI 3.1 |
| **Regulator** | Payroll consultants, HR specialists | No-Code Actions · C# Scripting |
| **Automator** | DevOps, integration engineers | .NET Client Services SDK · CLI |

## Quick Start

```sh
# 1. Login to GitHub Container Registry (one-time)
echo "<your-pat>" | docker login ghcr.io -u <github-username> --password-stdin

# 2. Clone and configure
git clone https://github.com/Payroll-Engine/PayrollEngine.git
cd PayrollEngine
echo "DB_PASSWORD=PayrollStrongPass789" > .env

# 3. Start
docker compose -f docker-compose.ghcr.yml up -d
```

Web Application: `http://localhost:8081` · Backend API: `http://localhost:5001`

→ [Full setup guide](https://payrollengine.org/GetStarted/ContainerSetup/)

## Repositories

| Repository | Description |
|:--|:--|
| [PayrollEngine](https://github.com/Payroll-Engine/PayrollEngine) | Main repo — Docker stack, examples, tests, schemas |
| [PayrollEngine.Backend](https://github.com/Payroll-Engine/PayrollEngine.Backend) | REST API server + SQL Server persistence |
| [PayrollEngine.WebApp](https://github.com/Payroll-Engine/PayrollEngine.WebApp) | Blazor web application |
| [PayrollEngine.PayrollConsole](https://github.com/Payroll-Engine/PayrollEngine.PayrollConsole) | CLI for automation, testing, and data import |
| [PayrollEngine.Client.Services](https://github.com/Payroll-Engine/PayrollEngine.Client.Services) | .NET Client SDK (NuGet entry package) |
| [PayrollEngine.Client.Scripting](https://github.com/Payroll-Engine/PayrollEngine.Client.Scripting) | Scripting API for regulation development |
| [PayrollEngine.Client.Core](https://github.com/Payroll-Engine/PayrollEngine.Client.Core) | Client core objects |
| [PayrollEngine.Client.Test](https://github.com/Payroll-Engine/PayrollEngine.Client.Test) | Test runner library |
| [PayrollEngine.Core](https://github.com/Payroll-Engine/PayrollEngine.Core) | Core payroll objects |
| [PayrollEngine.Document](https://github.com/Payroll-Engine/PayrollEngine.Document) | Report generation |
| [PayrollEngine.Serilog](https://github.com/Payroll-Engine/PayrollEngine.Serilog) | Structured logging |

→ [Full repository map](https://payrollengine.org/Resources/Repositories/)

## License

MIT — free for any use. See [LICENSE](https://github.com/Payroll-Engine/PayrollEngine/blob/main/LICENSE).
