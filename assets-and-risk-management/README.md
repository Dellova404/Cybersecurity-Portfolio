# Home Network Asset Inventory & Classification

## 📌 Contexto
Inventário prático de ativos e classificação de sensibilidade em ambiente de Home Office, seguindo as diretrizes do **NIST Cybersecurity Framework (Função Identify - ID.AM)**.

> *"Você só pode proteger o que sabe que tem."*

## 🎯 Objetivo
Identificar dispositivos conectados à rede local, avaliar criticidade, volume de acesso e nível de exposição a riscos, classificando os ativos para priorizar controles de segurança da informação.

## 🛠️ Ativos Mapeados e Classificação
* **Work Laptop (Confidencial):** Dispositivo corporativo dedicado que processa dados sensíveis da empresa. Protegido por controles de acesso estritos e uso exclusivo.
* **Network Printer (Interno):** Ativo local conectado via cabo. Monitorado devido a buffers de impressão (*spooling*) que processam documentos internos.
* **Smart TV / IoT (Interno):** Dispositivo de consumo doméstico. Embora não processe dados críticos, representa um vetor de risco de movimentação lateral (*pivot*) caso não esteja em uma VLAN isolada.

## 📄 Documentação Completa
O relatório detalhado com a planilha de controle e notas de segurança está disponível no arquivo:
👉 [Download do Inventário em PDF](./Home_Network_Asset_Inventory.pdf)
