# MLI-Knot-WinDiag Showcase

> **Status:** public sanitized showcase of a private/local Windows diagnosis, maintenance and recovery platform.  
> **Source project:** `MLI-Knot-WinDiag`, kept private/local.  
> **Safety posture:** read before write, preview before maintenance, reversible actions where supported, and explicit gates for higher-risk operations.

![Status](https://img.shields.io/badge/status-public%20showcase-blue)
![Baseline](https://img.shields.io/badge/baseline-0.1%20Foundation-brightgreen)
![Safety](https://img.shields.io/badge/default-read--only-darkgreen)
![Source](https://img.shields.io/badge/source%20project-private-orange)
![GitHub stars](https://img.shields.io/github/stars/proftectiagocosta-hash/MLI-Knot-WinDiag-Showcase?style=flat&label=stars)
![README views](https://hits.sh/github.com/proftectiagocosta-hash/MLI-Knot-WinDiag-Showcase.svg?label=README%20views)
![Language](https://img.shields.io/badge/language-PT--BR%20%7C%20EN-informational)

---

<div align="center">

<img src="assets/matrix-inspired-banner.gif" width="100%" alt="MLI-Knot cyber banner" />

</div>

---

## Português

### O que é

**MLI-Knot-WinDiag Showcase** é a superfície pública e sanitizada do projeto privado **MLI-Knot-WinDiag**.

A baseline privada `0.1.0` implementa uma plataforma de diagnóstico e manutenção do Windows com três direções documentadas de operação: uso local no Windows instalado, arquitetura remota autorizada e desativada por padrão, e suporte de recuperação offline orientado a WinPE.

O projeto não é apresentado como um simples conjunto de scripts. A base reúne orquestração de diagnóstico, API local e dashboard, CLI, coletores específicos do Windows, limpeza controlada, auditoria de inicialização do Registro, descoberta de atualizações, relatórios e componentes de recuperação.

### Capacidades implementadas na baseline

A fonte privada documenta e materializa:

- diagnóstico de sistema, hardware, armazenamento, rede, serviços, eventos, políticas, Registro, drivers e firmware;
- API local e dashboard no navegador;
- CLI para diagnóstico e operações previstas pela baseline;
- jobs assíncronos de diagnóstico com acompanhamento de progresso;
- geração de relatórios JSON e HTML;
- limpeza com preview, dry-run, regras de escopo, quarentena e restauração;
- auditoria de inicialização do Registro com fluxo reversível de disable/restore;
- inventário de drivers e firmware e descoberta de candidatos via Windows Update;
- assets e scripts para ambiente de recuperação WinPE;
- arquitetura remota preparada, mas local-only e desativada por padrão na configuração inicial.

### Evidência de validação registrada

A documentação da fonte registra uma validação real da baseline em Windows:

- solução compilada em **Release**;
- projetos Core, Windows, CLI, App e SmokeTests compilados;
- **smoke tests aprovados**;
- auditoria estrutural aprovada no checkpoint registrado;
- resolvedor robusto do SDK `.NET` validado;
- logs automáticos de build e teste funcionando no checkpoint registrado.

Em documentação posterior da mesma baseline, os scripts de build/teste foram corrigidos para preservar também a saída nativa completa e datada.

O ambiente experimentalmente validado registrado foi **Windows 10 Pro 22H2 x64, PowerShell 5.1 e .NET SDK 10.0.302**.

Essa evidência comprova operabilidade da baseline naquele ambiente. Ela **não transforma esse ambiente em plataforma oficialmente suportada**, não substitui a matriz de validação planejada e não constitui certificação de produção.

A documentação do projeto define como alvo oficial de desenvolvimento Windows 11 x64 e edições Windows 10 Enterprise/LTSC compatíveis com o runtime/SDK adotado.

### Modelo de segurança

O produto segue princípios conservadores:

- observar antes de alterar;
- separar diagnóstico de operações de escrita;
- exigir preview antes de manutenção;
- preferir quarentena ou desativação a exclusão;
- preservar possibilidade de restauração quando suportada;
- manter exposição remota desativada por padrão;
- não realizar flashing genérico de BIOS/UEFI ou firmware;
- não instalar drivers apenas porque foram descobertos.

A arquitetura remota existe como direção técnica, mas operação remota de produção exige gates adicionais de transporte, identidade, autorização, auditoria e recuperação.

### Estado do roadmap

O estado público correto é qualitativo, não um percentual arbitrário:

```text
0.1 Foundation        implemented
0.2 Stabilization     next
0.3 Controlled repair planned
0.4 OEM adapters      planned
0.5 Remote management planned
1.0 Stable product    gated future release
```

A antiga representação `1/6 = 16,7%` era apenas uma divisão matemática de marcos com pesos iguais. Ela não é uma métrica definida pela fonte para esforço, maturidade ou prontidão e, por isso, não é usada como indicador principal nesta vitrine.

### O que ainda não está provado

A baseline atual não autoriza afirmar:

- prontidão para produção;
- validação completa em toda a matriz Windows 10/11;
- cobertura universal de hardware, OEMs, drivers ou firmware;
- flashing automático e genérico de firmware;
- implantação remota de produção pronta;
- WinPE validado em uma matriz ampla de hardware;
- conclusão dos gates de estabilização, recuperação, threat model e release 1.0.

### Fronteira pública

Esta vitrine publica propósito, arquitetura em alto nível, capacidades, princípios de segurança, evidência técnica sanitizada, estado do roadmap e limitações.

Ela não publica código-fonte privado, credenciais, chaves, relatórios reais de máquinas, identificadores operacionais, logs internos, dados de quarentena/restauração, configurações privadas de implantação ou artefatos internos de continuidade.

Documentos históricos da fonte podem registrar decisões de sincronização já superadas. A vitrine segue o estado atual comprovado e não transforma documentação histórica em verdade operacional presente.

### Documentação

- [`docs/overview.md`](docs/overview.md)
- [`docs/public-boundary.md`](docs/public-boundary.md)
- [`docs/project-status.md`](docs/project-status.md)
- [`docs/roadmap.md`](docs/roadmap.md)
- [`assets/screenshots/README.md`](assets/screenshots/README.md)

---

## English

### What it is

**MLI-Knot-WinDiag Showcase** is the public sanitized surface of the private **MLI-Knot-WinDiag** project.

The private `0.1.0` baseline is a Windows diagnosis, controlled-maintenance and recovery platform. It combines local diagnostic orchestration, a local API/dashboard, CLI operation, Windows-specific collectors, reporting, reversible maintenance workflows, update discovery and WinPE-oriented recovery assets.

### Recorded validation

The source documentation records a real Windows validation in which the solution was built in **Release**, the Core, Windows, CLI, App and SmokeTests projects compiled, and the **smoke tests passed**.

The recorded experimental environment was **Windows 10 Pro 22H2 x64, PowerShell 5.1 and .NET SDK 10.0.302**.

This proves baseline operability in that recorded environment. It is not a production-readiness claim and does not redefine the project's officially documented support target.

### Current roadmap state

```text
0.1 Foundation        implemented
0.2 Stabilization     next
0.3 Controlled repair planned
0.4 OEM adapters      planned
0.5 Remote management planned
1.0 Stable product    gated future release
```

This showcase does not use an equal-weight milestone percentage as an engineering-progress metric.

### Safety and limits

Diagnosis and discovery are separated from write operations. Remote exposure is disabled by default, generic firmware flashing is outside the baseline automation model, and discovery of an update does not itself authorize installation.

Production readiness, broad hardware/OEM validation, production remote operation and the full 1.0 release gates remain unproven.

---

## Public status

```text
Repository type: public sanitized showcase
Source project: MLI-Knot-WinDiag
Source visibility: private/local
Current baseline: 0.1.0 Foundation
Foundation implementation: present
Recorded Windows Release build: passed
Recorded smoke tests: passed
Experimentally validated environment: Windows 10 Pro 22H2 x64 / PowerShell 5.1 / .NET SDK 10.0.302
Next roadmap milestone: 0.2 Stabilization
Production readiness claimed: no
Default remote exposure: disabled
Generic firmware flashing: not part of baseline automation
Private source code included: no
Sensitive operational material included: no
```
