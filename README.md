# Miniguia de Estudos: Mastering Cloud Architecture with NotebookLM

## 🎯 Contexto
Este repositório faz parte de um desafio prático utilizando o Google NotebookLM para sintetizar conhecimentos avançados sobre **arquitetura de nuvem**. O objetivo é consolidar frameworks de grandes provedores (AWS, Azure, Google Cloud), definições padronizadas pelo NIST e padrões de design agnósticos para formar um currículo de estudo sólido voltado para a carreira de **Arquiteto de Nuvem em 2026**.

## 📚 Curadoria de Fontes
| Fonte | Tipo | Descrição |
| :--- | :--- | :--- |
| **NIST Definition of Cloud Computing** | PDF | Define as características essenciais (autoatendimento, elasticidade, pooling de recursos) e modelos de serviço. |
| **Cloud Computing Design Patterns** | PDF | Catálogo técnico de padrões agnósticos para escalabilidade, confiabilidade e segurança. |
| **Azure/Google Architecture Frameworks** | Link | Melhores práticas focadas em pilares como Excelência Operacional e Otimização de Custos. |
| **Roadmap Cloud Engineer/AWS 2026** | Mídia | Guias práticos sobre o stack de habilidades (Linux, Redes, IaC) e o papel decisório do arquiteto. |

## 🧠 Engenharia de Prompts (Log de Experimentos)
> **Desafio encontrado:** A IA estava sendo muito genérica nos resumos, focando apenas em conceitos básicos.
> **Solução:** Implementei a técnica de *Chain-of-Thought* no prompt, solicitando que a IA primeiro diferenciasse o papel do executor (SysAdmin) do papel do arquiteto (tomador de decisão) antes de resumir os frameworks técnicos. Além disso, direcionei a análise para as tendências de 2026, como a integração de IA no pilar de Excelência Operacional.

## 📖 Miniguia de Estudo

### Resumo Executivo
A arquitetura de nuvem em 2026 exige que o profissional evolua de um configurador de serviços para um **tomador de decisões estratégicas**. O papel central do arquiteto é justificar o "porquê" de cada escolha técnica, equilibrando ganhos e perdas (trade-offs) entre custo, performance e disponibilidade.

Os principais frameworks (AWS, Azure, Google) convergem em pilares fundamentais:
*   **Confiabilidade e HA (Alta Disponibilidade):** Garantir que o sistema opere sem interrupções através de redundância e mecanismos de *failover*.
*   **Segurança:** Proteção em camadas, utilizando perímetros definidos logicamente e controles de acesso rigorosos.
*   **Otimização de Custos:** Evitar o desperdício pagando apenas pelo que é utilizado, empregando escalabilidade elástica e instâncias reservadas ou spot.
*   **Modernização:** O uso de **Multi-Cloud** para evitar o bloqueio por fornecedor (*vendor lock-in*) e a adoção de **Containers (Kubernetes)** e **Serverless** para aumentar a agilidade operacional.

### Glossário
*   **Escalabilidade Horizontal:** Adição de mais instâncias de recursos (como servidores) para distribuir a carga.
*   **Elasticidade Rápida:** Capacidade de expandir ou reduzir recursos computacionais automaticamente conforme a demanda.
*   **Resource Pooling:** Agrupamento de recursos físicos e virtuais para atender múltiplos consumidores de forma dinâmica.
*   **Disaster Recovery (DR):** Estratégias para restaurar sistemas e dados após eventos catastróficos, focando em backup e replicação.
*   **Infrastructure as Code (IaC):** Prática de provisionar e gerenciar infraestrutura através de código (ex: Terraform), garantindo reprodutibilidade.

### Prompts Recomendados
- "Analise as fontes e crie um quiz de 5 perguntas sobre as diferenças técnicas entre **High Availability (HA)** e **Disaster Recovery (DR)** em ambientes Multi-Cloud".
- "Com base no Roadmap 2026, descreva os 3 projetos de portfólio ideais para demonstrar experiência real sem estar empregado".
- "Explique o padrão de design **Hypervisor Clustering** e como ele previne falhas em cascata em servidores virtuais".
- "Crie um guia passo a passo para implementar uma arquitetura de três camadas na AWS, incluindo segurança e observabilidade".
