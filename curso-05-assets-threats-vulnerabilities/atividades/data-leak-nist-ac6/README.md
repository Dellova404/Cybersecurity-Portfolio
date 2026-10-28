# 🛡️ Data Leak Analysis & Remediation (NIST SP 800-53: AC-6)

## 📌 Contexto
Análise de incidente de vazamento de dados (*data leak*) em uma empresa de tecnologia educacional, decorrente de falhas no controle de acesso e erro humano no compartilhamento de arquivos confidenciais com parceiros externos.

Atividade prática desenvolvida no **Google Cybersecurity Professional Certificate** (Curso 5: *Assets, Threats, and Vulnerabilities*), alinhada ao framework **NIST CSF** (Função: **Protect [PR.DS-5]**) e aos controles de acesso **NIST SP 800-53: AC-6**.

---

## 🎯 Objetivo
Avaliar os fatores de risco que causaram a exposição acidental de planos de negócios internos, mapear os requisitos da norma **NIST AC-6 (Principle of Least Privilege)** e recomendar melhorias técnicas para impedir a reincorrência do incidente.

---

## 🔍 Resumo do Incidente
* **Causa Raiz:** Um gestor compartilhou uma pasta interna contendo arquivos confidenciais e métricas de clientes com a equipe de vendas e não revogou o acesso ao término da reunião (*privilege creep* / acesso residual).
* **Falha Humana & Técnica:** Durante uma conferência com parceiro externo, um colaborador compartilhou por engano o link da pasta inteira em vez de apenas o material promocional, culminando na publicação dos documentos internos em redes sociais.

---

## 📋 Matriz de Resposta (Data Leak Worksheet)

| Campo | Análise & Justificativa Técnica |
| :--- | :--- |
| **Issue(s)** | A chain of access failures led to the data leak. First, the manager granted access to confidential internal folders and failed to revoke it after the meeting. Subsequently, the sales representative mistakenly shared the entire root folder with an external partner due to a lack of technical restrictions on outbound links. |
| **Review (NIST AC-6)** | NIST SP 800-53: AC-6 addresses the principle of least privilege. It establishes that organizations must limit user and process authorizations strictly to the minimum access required to execute specific business functions. This prevents accounts from operating with elevated, unneeded permissions. |
| **Recommendation(s)** | **1. Automatically revoke access:** Implement automatic expiration policies that revoke temporary access to sensitive internal folders after a set time frame.<br>**2. Regularly audit user privileges:** Conduct routine privilege audits to ensure permissions align with active job roles and immediately eliminate unused authorizations. |
| **Justification** | Implementing automated access revocation eliminates human error by ensuring lingering permissions are not left active when managers forget to unshare resources. Additionally, routine privilege audits verify compliance with least privilege, drastically reducing the likelihood of unauthorized external data exposure. |

---

## 💡 Competências Aplicadas
* **Princípio do Menor Privilégio (PoLP):** Implementação de regras restritivas de autorização e mitigação de *privilege creep*.
* **Governança e Controles de Acesso:** Aplicação prática dos catálogos de controles de segurança **NIST SP 800-53** e alinhamento com a categoria de proteção de dados do **NIST CSF**.
* **Gestão de Vazamento de Dados (DLP):** Recomendações de políticas de expiração de acessos temporários e bloqueio técnico de links para domínios externos.

---

## 📄 Arquivo da Atividade
👉 [Download da Planilha de Análise em PDF](./Data_Leak_Worksheet.pdf)
