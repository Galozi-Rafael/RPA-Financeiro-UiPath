# RPA Financeiro com UiPath

Automação desktop do aplicativo **Money Manager Ex** utilizando **UiPath**.

O objetivo deste projeto é automatizar processos operacionais dentro de um software financeiro desktop, simulando interações humanas na interface gráfica da aplicação.

---

# Tecnologias Utilizadas

- UiPath Studio
- UI Automation
- Windows Desktop Automation
- CSV (importação e exportação de dados)

---

# Objetivo do Projeto

Automatizar tarefas repetitivas no aplicativo **Money Manager Ex**, como criação de base de dados e manipulação de transações financeiras.

A automação interage diretamente com a interface do software, identificando elementos da UI através das ferramentas de inspeção do **UiPath** e controlando o aplicativo através das atividades de automação.

---

# Funcionalidades Automatizadas

Atualmente a automação executa os seguintes processos:

### 1. Criação de nova base de dados
- Abre o aplicativo Money Manager Ex
- Navega pelo assistente de criação de banco de dados
- Define o local e nome do arquivo

### 2. Configuração inicial da base
Configura automaticamente os parâmetros iniciais do sistema:

- Nome do usuário
- Moeda padrão
- Criação de conta inicial

### 3. Importação de transações
- Importa transações financeiras a partir de um arquivo `.csv`

### 4. Exportação de relatório
- Gera relatório financeiro
- Exporta os dados para arquivo `.csv`

---

# Estrutura do Projeto

```mermaid
flowchart LR

A[RPA Financeiro] --> B[RPAFinanceiro]
A-->C[.gitignore]
A-->D[README.md]

B-->E[cases]
B-->F[Servs]
B-->G[data] --> H[input]
H-->I[output]
H-->J[main.xaml]