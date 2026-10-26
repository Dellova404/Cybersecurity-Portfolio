# 🏦 Commercial Bank Risk Assessment & Risk Register

## 📌 Contexto
Simulação prática de avaliação de riscos e preenchimento de **Risk Register (Registro de Riscos)** para um banco comercial com equipe híbrida (120 colaboradores) e conformidade com órgãos reguladores (Federal Reserve / Banco Central).

Atividade desenvolvida no âmbito do programa profissional **Google Cybersecurity Certificate**, alinhada à função **Identify (ID.RA - Risk Assessment)** do NIST CSF.

## 🎯 Objetivo
Avaliar vulnerabilidades e ameaças à integridade, confidencialidade e disponibilidade dos fundos bancários e dados de clientes, calculando a matriz de risco para priorização de recursos de defesa.

## 📐 Metodologia de Cálculo
$$\text{Prioridade (Risco)} = \text{Probabilidade (Likelihood)} \times \text{Severidade (Severity)}$$

* **Probabilidade:** 1 (Baixa) a 3 (Alta)
* **Severidade:** 1 (Baixa) a 3 (Crítica)
* **Escala de Risco:** 1 a 9

## 📊 Matriz de Priorização de Riscos

| Risco Identificado | Probabilidade (1-3) | Severidade (1-3) | Pontuação (1-9) | Nível de Prioridade |
| :--- | :---: | :---: | :---: | :--- |
| **Compromised User Database** | 3 | 3 | **9** | **Crítica** |
| **Business Email Compromise (BEC)** | 2 | 3 | **6** | **Alta** |
| **Financial Records Leak** | 1 | 2 | **2** | **Moderada** |
| **Physical Theft** | 1 | 2 | **2** | **Baixa** |
| **Supply Chain Attack** | 1 | 1 | **1** | **Baixa** |

## 💡 Principais Conclusões
* **Foco Imediato de SOC:** O banco de dados de clientes e os ataques de engenharia social (BEC) receberam a prioridade máxima (9 e 6), demandando monitoramento contínuo de logs de autenticação, implementação rigorosa de MFA e regras de detecção de exfiltração em SIEM/EDR.
* **Ambiente Crítico:** Setores financeiros possuem tolerância quase nula a incidentes devido a exigências regulatórias rigorosas e impacto direto na reputação institucional.

## 📄 Documentação Completa
👉 [Download da Planilha de Riscos em PDF](./Risk_Register_Bank.pdf)
