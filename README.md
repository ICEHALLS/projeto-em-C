O processo utilizado foi:


### Passo 1: Criar um Repositório no GitHub

1. **Acesse o GitHub**: Entre no [site do GitHub](https://github.com) e faça login.

  
2. **Crie um Novo Repositório**:
   - Clique no botão **New** ou **Novo repositório** (geralmente está na barra lateral esquerda ou na sua página de perfil).
   - Dê um nome ao repositório, por exemplo, `projeto-em-C`.
   - Adicione uma descrição, como "Primeiro projeto em C usando Git e GitHub".
   - Escolha se quer o repositório **Público** (para que todos possam ver) ou **Privado**.
   - Não adicione arquivos como README ou .gitignore neste momento (vamos adicionar do seu projeto local).
   - Clique em **Create repository** para criar o repositório.

---

### Passo 2: Configurar o Repositório Localmente no Git Bash

1. **Abra o Git Bash** na pasta onde você colocou o projeto em C.
   - Navegue até a pasta do seu projeto. Por exemplo:

     ```bash
     cd caminho/para/sua/pasta/de/teste
     ```

2. **Inicialize o Git na Pasta do Projeto**:

   ```bash
   git init
   ```

   Isso cria um repositório Git vazio na pasta. Agora você pode começar a rastrear arquivos.

---

### Passo 3: Adicionar e Comitar os Arquivos do Projeto

1. **Adicionar Todos os Arquivos**:
   
   ```bash
   git add .
   ```

   O ponto `.` significa "adicionar todos os arquivos no diretório atual".

2. **Fazer o Primeiro Commit**:

   ```bash
   git commit -m "Primeiro commit: Adiciona projeto em C"
   ```

   Esse comando cria um commit, ou seja, uma "foto" do estado atual do seu projeto, com a mensagem "Primeiro commit: Adiciona projeto em C".

---

### Passo 4: Conectar o Repositório Local ao Repositório do GitHub

1. **Adicionar o Repositório Remoto**:
   - Copie a URL do repositório que você acabou de criar no GitHub. Ela deve ter o formato `https://github.com/seu-usuario/projeto-em-C.git`.
   - No Git Bash, execute:

     ```bash
     git remote add origin https://github.com/seu-usuario/projeto-em-C.git
     ```

     Substitua `https://github.com/seu-usuario/projeto-em-C.git` pela URL real do seu repositório.

2. **Enviar os Arquivos para o GitHub**:

   ```bash
   git push -u origin master
   ```

   Esse comando envia seu commit para o GitHub na branch `master` (ou `main`, se você estiver usando essa nomenclatura).

---

### Passo 5: Verificar no GitHub

1. Vá para a página do seu repositório no GitHub.
2. Atualize a página, e você deve ver os arquivos do seu projeto em C agora no repositório!

---

### Passo 6: Adicionar um README (Opcional, mas Recomendado)

Um arquivo `README.md` é útil para descrever o que seu projeto faz. Você pode adicionar um arquivo README para explicar o propósito do projeto, como executá-lo, e quaisquer outras informações.

1. Crie um arquivo chamado `README.md` na sua pasta do projeto.
2. Adicione algumas informações, como:

   ```markdown
   # Projeto em C

   Este é meu primeiro projeto em C usando Git e GitHub.

   ## Como Compilar

   ```bash
   gcc nome_do_arquivo.c -o nome_do_programa
   ./nome_do_programa
   ```
   ```

3. Salve o arquivo e envie para o GitHub:

   ```bash
   git add README.md
   git commit -m "Adiciona README"
   git push
   ```

---

