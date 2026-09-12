# MLI-Knot-WinDiag Showcase

> **Status:** public sanitized showcase of a private/local Windows diagnosis, maintenance and recovery platform.  
> **Source project:** `MLI-Knot-WinDiag`, kept private/local.  
> **Safety model:** diagnosis is read-only by default; potentially destructive operations remain bounded, reversible or explicitly gated.

![Status](https://img.shields.io/badge/status-public%20showcase-blue)
![Roadmap](https://img.shields.io/badge/documented%20roadmap-16.7%25-yellow)
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

O projeto fonte reúne diagnóstico do Windows, manutenção controlada, limpeza segura, auditoria do Registro, inventário de drivers e firmware, descoberta de atualizações, relatórios, operação remota preparada e suporte de recuperação por WinPE.

O desenho é deliberadamente conservador: diagnóstico é somente leitura por padrão, limpeza usa prévia/quarentena/restauração, alterações de Registro são reversíveis e firmware não é atualizado por automação genérica.

### Capacidades representadas

A base atual documenta:

- motor de diagnóstico local;
- API local e dashboard;
- CLI;
- inventário de sistema, hardware, armazenamento, rede, serviços, eventos, políticas, Registro, drivers e firmware;
- descoberta de atualizações aplicáveis;
- limpeza segura com preview, dry-run, quarentena, recibos e restauração;
- auditoria de inicialização do Registro com disable/restore;
- relatórios JSON e HTML;
- jobs assíncronos de diagnóstico;
- builder de WinPE e diagnóstico offline;
- arquitetura remota preparada, desativada por padrão.

### Marcador de progresso

O roadmap fonte possui **6 marcos nomeados**:

`0.1 Foundation`, `0.2 Stabilization`, `0.3 Controlled repair`, `0.4 OEM adapters`, `0.5 Remote management` e `1.0 Stable product`.

O marco **0.1 Foundation** está documentado como implementado.

**Marcador público por contagem de marcos documentados: 1/6 = 16,7%.**

Esse percentual mede somente **marcos nomeados do roadmap com peso unitário**. Ele não estima esforço de engenharia, quantidade de código, maturidade de segurança ou prontidão de produção. Os marcos possuem complexidades diferentes.

### Estado e próximos passos

A fundação funcional existe, mas o roadmap ainda prevê estabilização em Windows, proteção adicional de credenciais locais, recibos assinados, reparos controlados, adapters OEM, maturidade remota e os gates necessários para uma versão 1.0 estável.

### Limites públicos

Esta vitrine não publica:

- código-fonte privado;
- chaves locais, credenciais ou dados de runtime;
- logs operacionais;
- relatórios reais de máquinas;
- nomes de usuários, máquinas ou ambientes;
- IPs, gateways, identificadores de hardware ou dispositivos reais;
- quarentenas, backups ou artefatos de restauração reais;
- checkpoints internos;
- configurações privadas de implantação;
- procedimentos que enfraqueçam os gates de segurança.

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

The source project combines Windows diagnostics, controlled maintenance, safe cleanup, Registry auditing, driver and firmware inventory, update discovery, reporting, remote-ready architecture and WinPE recovery support.

The design is intentionally conservative: diagnosis is read-only by default, cleanup is reversible, Registry remediation is controlled and generic firmware flashing is not part of the automation model.

### Progress marker

The documented roadmap contains six named milestones. The `0.1 Foundation` milestone is implemented.

**Public roadmap milestone-count marker: 1/6 = 16.7%.**

This is an equal-weight count of named roadmap milestones, not an engineering-effort or production-readiness estimate.

### Public boundary

Only sanitized documentation, fictional examples, public-safe diagrams and deliberately prepared screenshots belong here.

Private source code, real machine reports, operational identifiers, credentials, local runtime material and internal continuity artifacts remain private.

---

## Public status

```text
Repository type: public sanitized showcase
Source project: MLI-Knot-WinDiag
Source visibility: private/local
Documented roadmap milestones: 6
Completed named milestones: 1
Roadmap milestone-count marker: 16.7%
Engineering effort completion claimed: no
Production readiness claimed: no
Default diagnosis mode: read-only
Private source code included: no
Sensitive operational material included: no
```
