# 🔐 Escape Room DevOps 3 — Infra Comprometida

Bem-vindo ao desafio **Escape Room DevOps 3**
Sua missão é investigar uma infraestrutura comprometida e recuperar uma **A frase que está perdida** e escondida em diferentes camadas do sistema.

---

## 🧠 Contexto

Nossa infraestrutura foi comprometida e informações críticas foram espalhadas em:

- 📂 Histórico do Git
- 🐳 Containers Docker
- ⚙️ Pipeline de CI/CD

Seu objetivo é **recuperar todas as partes da frase** e montar a mesma.

---


---

# 🧩 Tarefa 1 — Investigação no Git

Nosso primeiro objetivo é encontrar as palavras perdidas no histórico do repositório.

### 📌 Desafios:

- Crie uma branch contendo os **3 commits perdidos**
- Encontre os arquivos que possuem partes da frase
- Os valores estão em **base64**

### 🧪 Dica:

Use o comando:

- bash echo "valor_encontrado" | base64 -d

---


# 🐳 Tarefa 2 — Container Comprometido

Agora precisamos analisar o ambiente Docker.

### 📌 Objetivos:

- Use o script `.sh` para subir o ambiente
- Corrija o `Dockerfile` se necessário
- Faça a aplicação funcionar corretamente

### 🔍 Investigação:

- Descubra as palavras exposta pela API
- Encontre **duas palavras escondidas dentro do container**

# ⚙️ Tarefa 3 — CI/CD Quebrado

A última parte da frase está no pipeline de integração contínua.

### 📌 Objetivos:

- Corrigir o workflow de CI/CD
- Fazer o pipeline executar corretamente
- Identificar e configurar variáveis necessárias

### 🔍 Investigação:

- Analise o arquivo `.github/workflows`
- Identifique erros no pipeline
- Descubra quais variáveis precisam ser criadas no repositório

### 🔐 Importante:

- A flag **não estará em texto claro**
- Ela será gerada no final do pipeline de forma **criptografada**
- Você precisará interpretar o resultado final

### 🧪 Dicas:

```bash
- Verifique os logs da execução do GitHub Actions
- Procure por erros de configuração
- Fique atento a variáveis não definidas
- Identifique saídas codificadas (ex: base64)