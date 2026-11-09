# implementando-monitoramento-no-azure
Documentação prática, resumos e guia de configuração sobre monitoramento de recursos e diagnósticos no Microsoft Azure (Azure Monitor, Log Analytics e Network Watcher).

# Implementando Monitoramento no Microsoft Azure ☁️📊

Este repositório contém a documentação completa, resumos práticos e guias técnicos desenvolvidos durante o laboratório **"Implementando Monitoramento no Azure"**. O objetivo deste projeto é demonstrar como manter visibilidade, controle e resposta proativa sobre eventos críticos em infraestruturas de nuvem.

---

## 📌 Objetivos do Projeto
- **Monitoramento contínuo:** Entender a diferença e aplicação de **Métricas** e **Logs**.
- **Alertas Automatizados:** Estruturar regras de alertas e **Grupos de Ação** (*Action Groups*).
- **Análise de Dados:** Centralização de telemetria no **Log Analytics Workspace** e consultas com **KQL**.
- **Diagnóstico Avançado:** Monitoramento de rede com **Network Watcher** em Máquinas Virtuais (VMs).

---

## 🧠 Principais Conceitos e Aprendizados

### 1. Azure Monitor: Métricas vs. Logs
- **Métricas:** Dados numéricos leves coletados em tempo real (ex: % de uso de CPU, memória disponível, tráfego de rede). Ideal para alertas rápidos de desempenho.
- **Logs:** Registros detalhados e estruturados armazenados em tabelas de um *Log Analytics Workspace*. Permite auditoria profunda e diagnósticos complexos via consultas KQL.

### 2. Fluxo de Criação de Regras de Alerta
1. **Escopo/Recurso:** Seleção da VM, grupo de recursos ou assinatura a ser monitorada.
2. **Condição:** Definição do sinal (métrica ou log) e do limite de disparo.
3. **Grupo de Ação (Action Group):** Definição das ações automatizadas (notificação por e-mail/SMS, webhooks ou scripts).
4. **Detalhes e Ativação:** Configuração da severidade e habilitar a regra de monitoramento.

### 3. Log Analytics e Consultas KQL
- **Log Analytics Workspace:** Repositório central onde os logs são agregados e consolidados.
- **Syslog (Linux) / Event (Windows):** Tabelas nativas para ingestão de eventos do sistema operacional.
- **Queries Prontas:** Utilização das consultas nativas da plataforma como base para auditoria, diagnóstico de falhas e análise de performance.

### 4. Diagnóstico de Infraestrutura e Segurança
- **Network Watcher:** Requer a *Extensão VM do Agente Observador de Rede* para capturar pacotes e diagnosticar problemas de conectividade em máquinas virtuais.
- **Activity Log (Categoria Administrativo):** Registro utilizado para auditar ações na infraestrutura (como a exclusão inadvertida ou programada de recursos e NSGs).

---

## 🛠️ Estrutura do Repositório
```text
.
├── README.md           # Documentação principal do projeto
└── /images             # Capturas de tela dos laboratórios e testes (opcional)
