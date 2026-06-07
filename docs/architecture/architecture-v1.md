# Architecture v1 - IT-IMRT

## Objetivo da versão 0.1

Definir a arquitetura inicial do projeto IT-IMRT, com foco no módulo de inventário de ativos, estrutura do backend, banco de dados SQLite e base para futura interface web.

## Escopo inicial

- Cadastro manual de ativos;
- Armazenamento em SQLite;
- Estrutura inicial em Python;
- Preparação para API com FastAPI;
- Organização do projeto para futuras funcionalidades de monitoramento.

## Módulos planejados

### Asset Inventory Module

Responsável pelo cadastro, consulta e organização dos ativos de TI.

### Monitoring Module

Responsável por verificações futuras de disponibilidade, inicialmente por ICMP.

### Reporting Module

Responsável pela geração futura de relatórios operacionais.

## Entidade inicial: Asset

Campos previstos:

- id
- hostname
- ip_address
- operating_system
- asset_type
- status
- created_at
- updated_at

## Fluxo inicial

Host / Ativo
↓
Cadastro no sistema
↓
Banco SQLite
↓
Consulta via interface web