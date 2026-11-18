# Sistema de Gestão de Férias (Spring Boot)

Sistema desenvolvido para automatizar e controlar o planejamento de férias de **gerentes e supervisores**, garantindo a operação contínua das lojas e o cumprimento das regras internas de folga.

---

## Funcionalidades Principais

* **🔐 Autenticação e Perfis:** Controle de acesso separado entre Usuários Comuns (Gerentes/Supervisores) e Administradores.
* **📅 Calendário de Férias:** Visualização anual (até 2028) integrando o período de férias do próprio usuário e dos colegas pares.
* **⚡ Regras de Conflito Inteligentes:**
  * Cargos iguais na mesma loja **não podem** tirar férias no mesmo período (bloqueio automático).
  * Gerentes de lojas diferentes podem tirar no mesmo período **desde que aprovados pelo Admin**.
* **✂️ Fracionamento de Férias:** Controle dinâmico do saldo e dos períodos fracionados (respeitando o limite de 30 dias anuais).
* **🔄 Fluxo de Aprovação:**
  * O primeiro agendamento de férias segue direto.
  * Solicitações de alteração ou exclusão após o primeiro cadastro exigem aprovação prévia do Admin (com notificações).
* **✉️ Alertas Automáticos por E-mail:** Disparo de lembretes automáticos para o usuário e o administrador faltando **30 dias** e **5 dias** para o início das férias.
* **👑 Painel do Administrador:** Gestão completa de usuários, visualização de férias vencidas/proporcionais, aprovações pendentes e histórico.

---

## 🛠️ Tecnologias Utilizadas

* **Java 17+**
* **Spring Boot** (Core, Web, Security)
* **Spring Data JPA / Hibernate** (Mapeamento ORM e Banco de Dados)
* **Spring Mail** (Envio de e-mails transacionais)
* **Maven** (Gerenciador de dependências)
* **Banco de Dados Relacional** (MySQL / PostgreSQL)

---

## ⚙️ Como Executar o Projeto

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/devflucassilva-byte/Sistema_ferias.git](https://github.com/devflucassilva-byte/Sistema_ferias.git)
