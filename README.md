# 📋 **Sistema de Gestão de Demandas**

Este sistema é uma plataforma de gestão de demandas com autenticação de usuários, funcionalidades de gestão e análise de tarefas, focado em facilitar o acompanhamento e a execução das demandas dentro de uma organização. 

## 🚀 **Funcionalidades**

### 1. 🔑 **Sistema de Login**
O sistema implementa um processo de autenticação com diferentes tipos de usuários. Existem dois tipos de usuários:

- 👩‍💼 **Líder**: Tem permissões avançadas, incluindo a possibilidade de **confirmar ou devolver** demandas.
- 👨‍💻 **Colaboradores**: Podem visualizar e gerenciar suas próprias demandas.

Cada usuário tem informações específicas, como:
- **Senha** 🔒
- **Cargo** 🏷️
- **Outras informações** 📝

A autenticação é gerenciada através do `st.session_state`, que mantém o estado do login durante a interação com o sistema.

---

### 2. 📝 **Gestão de Demandas**
Os usuários podem criar novas demandas com as seguintes informações:

- **Título** 📛: Nome da demanda.
- **Descrição** 📝: Detalhamento da tarefa ou solicitação.
- **Tipo de demanda** 📊: Classificação da demanda (ex: Técnico, Administrativo, etc.).
- **Prioridade** ⚠️: Nível de urgência (ex: Alta, Média, Baixa).
- **Data limite** 📅: Prazo para conclusão da demanda.

As demandas são atribuídas a **colaboradores específicos** 👨‍💻👩‍💻, que irão gerenciá-las conforme o progresso.

---

### 3. 🗂️ **Interface com Abas**
O sistema é dividido em 4 abas principais:

- 🏠 **Minhas Demandas**: Mostra todas as demandas associadas ao usuário logado.
- ✅ **Confirmar Conclusão**: Exclusiva para o líder, onde ele pode confirmar ou devolver demandas.
- 📜 **Histórico**: Registro de todas as atividades realizadas no sistema.
- 📊 **Dashboard**: Área com métricas e análises detalhadas.

---

### 4. 🧑‍💼 **Funcionalidades por Aba**

#### **Minhas Demandas** 🔍
- **Filtros** 🔘 para **status**, **prioridade** e **tipo** de demanda.
- Opção de **marcar demandas como concluídas** ✅.
- **Visualização detalhada** 🧐 de cada demanda.

#### **Confirmar Conclusão** ✔️
- Exclusiva para o **líder** 👑.
- Permite **confirmar ou devolver** demandas 🔄.
- **Adicionar observações** 📝 durante o processo de confirmação.

#### **Histórico** 📚
- Registro completo de todas as ações realizadas 📑.
- **Filtros** 🔎 por **usuário** e **tipo** de ação.
- **Visualização cronológica** 📅 das atividades.

#### **Dashboard** 📈
- **Métricas gerais** 📊 sobre o progresso das demandas.
- **Desempenho por colaborador** 🧑‍💻📊.
- **Análise por tipo de demanda** 📊.
- **Geração de relatórios** 📑.

---

### 5. ⚙️ **Recursos Adicionais**
- **Sistema de notificações** 🔔 para alertar os usuários sobre atualizações nas demandas.
- **Botão de logout** 🚪 para encerrar a sessão.
- **Geração de relatórios em CSV** 📤 para exportar dados relevantes.
- Interface **responsiva** 📱💻 criada com o Streamlit, garantindo uma boa experiência em diferentes dispositivos.

---

Este sistema visa melhorar a organização e a produtividade dentro das equipes, permitindo um acompanhamento eficiente das demandas e facilitando a comunicação entre líderes e colaboradores. 👏
