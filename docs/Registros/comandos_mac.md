# 📜 Comandos Básicos para Gerenciar a Memória Digital no Mac

> **Registro 005: Comandos Essenciais para Terminal e MkDocs**  
> 📅 **Data:** 2025  
> ✍️ **Autores:** João & Léo  

---

## 🖥️ 1. **Acessando o Diretório da Memória Digital**

Antes de qualquer ação, precisamos navegar até a pasta onde está o projeto.

```sh
# Abrir o terminal e entrar no diretório correto
cd ~/Documents/MemoriaDigital
```

Verificar se estamos no diretório correto:

```sh
pwd  # Exibe o caminho completo do diretório atual
ls   # Lista os arquivos e pastas dentro do diretório atual
```

Caso precise voltar um nível:

```sh
cd ..   # Volta para a pasta anterior
```

---

## 📂 2. **Visualizar Arquivos e Estrutura**

Listar os arquivos dentro do diretório `MemoriaDigital`:

```sh
ls -R  # Lista todos os arquivos e subpastas de forma recursiva
```

Se quiser ver detalhes como permissões e tamanho:

```sh
ls -lh
```

Para abrir arquivos Markdown no VS Code:

```sh
code index.md  # Abre o arquivo index.md no VS Code
```

Caso `code` não funcione, abra o VS Code manualmente e use **File > Open Folder...** para abrir `MemoriaDigital`.

---

## 🚀 3. **Rodando o Servidor Local do MkDocs**

Para visualizar as mudanças antes de publicar, rodamos o servidor local:

```sh
mkdocs serve
```

Isso inicia um servidor acessível no navegador em:

🔗 **http://127.0.0.1:8000/**

Para desligar o servidor, pressione **CTRL + C** no terminal.

Se o terminal travar, feche a aba e abra um novo terminal para rodar os comandos novamente.

---

## 📡 4. **Publicando no GitHub Pages**

Depois de fazer edições e conferir no servidor local, podemos atualizar a versão online:

```sh
mkdocs gh-deploy
```

Isso faz o build e envia os arquivos para a branch `gh-pages` no GitHub. O site estará disponível em:

🔗 **https://joaoeleo.github.io/memoria-digital/**

Caso precise forçar a atualização:

```sh
mkdocs gh-deploy --clean --force
```

---

## 🔥 5. **Comandos Úteis do Git**

Verificar o status do repositório:

```sh
git status
```

Adicionar arquivos ao commit:

```sh
git add .
```

Criar um commit com mensagem:

```sh
git commit -m "Atualização da Memória Digital"
```

Enviar as mudanças para o GitHub:

```sh
git push origin main
```

Para alternar para a branch `gh-pages` (caso necessário):

```sh
git checkout gh-pages
```

E para voltar para a branch `main`:

```sh
git checkout main
```

---

## 🎯 6. **Próximos Passos**

✅ Verificar se todos os comandos funcionam corretamente no seu ambiente.
✅ Continuar expandindo os registros da Memória Digital com novos conteúdos.
✅ Melhorar a organização e aparência do site conforme necessário.

✍️ **Autores:** João & Léo  
📖 **Coautores e Resistentes na Fé**
