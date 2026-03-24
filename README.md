# 📝 Guia para contribuição #
___
## 🚀 Fluxo de Trabalho (Git Flow)
Para manter a organização e evitar conflitos no código, seguimos este padrão:

### 1. Branches Principais
*   `main`: Contém apenas o código estável e testado (versão de produção).
*   `develop`: Branch principal de desenvolvimento onde todas as novas funcionalidades são reunidas.

### 2. Como Contribuir
Sempre que for iniciar uma nova tarefa, siga estes passos:

1.  **Atualize sua base**:
    ```bash
    git checkout develop
    git pull origin develop
    ```
2.  **Crie uma branch para sua tarefa**:
    ```bash
    git checkout -b feature/nome-da-sua-tarefa
    ```
3.  **Desenvolva e faça o commit**:
    ```bash
    git add .
    git commit -m "Explique brevemente o que foi feito"
    ```
4.  **Suba sua branch e abra um Pull Request**:
    ```bash
    git push origin feature/nome-da-sua-tarefa
    ```

### ⚠️ Regras de Ouro
*   **Nunca** faça push direto na `main` ou na `develop`.
*   Toda funcionalidade deve passar por um **Pull Request (PR)**.
*   Pelo menos **1 colega** deve revisar o seu código antes do Merge para a `develop`.
___
## 📝 Padrão de Commits
Utilizamos o padrão **Conventional Commits** para um histórico limpo e profissional:

*   ✨ `feat`: Nova funcionalidade.
*   🐛 `fix`: Correção de bugs.
*   📝 `docs`: Mudanças na documentação.
*   🎨 `style`: Formatação, CSS ou estilo (sem mudar lógica).
*   ♻️ `refactor`: Refatoração de código existente.
*   ⚡ `perf`: Melhoria de performance.
*   ✅ `test`: Adição ou correção de testes.

### 💡 Exemplos de Commits para a Equipe, utilize estes modelos:
### ✨ feat (Nova funcionalidade)
- ✨ feat: adiciona sistema de login com Google
- ✨ feat: cria barra de busca na página inicial

### 🐛 fix (Correção de erros/bugs)
- 🐛 fix: corrige erro no cálculo do carrinho de compras
- 🐛 fix: resolve quebra de layout no Safari

### 🎨 style (Mudanças visuais ou de formatação)
- 🎨 style: altera cor do botão principal para azul
- 🎨 style: ajusta espaçamento entre os cards de produto

### ✅ test (Criação ou alteração de testes)
- ✅ test: adiciona teste de validação para campo de e-mail
- ✅ test: corrige falha no teste de integração da API

### 📝 docs (Documentação)
- 📝 docs: atualiza instruções de instalação no README
- 📝 docs: adiciona link do Figma no manual do projeto
### ♻️ refactor (Melhoria no código sem mudar o que ele faz)
- ♻️ refactor: simplifica a função de autenticação
- ♻️ refactor: remove variáveis não utilizadas no componente Header
