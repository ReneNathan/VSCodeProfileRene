# Perfil de Usuário do Visual Studio Code

Este repositório contém o perfil de configurações do Visual Studio Code com foco em desenvolvimento web moderno e Python. As preferências foram ajustadas para proporcionar uma experiência mais produtiva, com destaque para organização, formatação de código e usabilidade.

## ✨ Principais Características

- **Formatação automática ao salvar**
- **Uso do Prettier como formatador padrão**
- **Linting com ESLint para JavaScript e TypeScript**
- **Ambiente ideal para desenvolvimento com React, Tailwind e Python**
- **Suporte a ícones de arquivos e temas visuais personalizados**
- **Autoimportação e ordenação de imports com isort (Python)**

---

## ⚙️ Extensões Recomendadas

> Estas extensões são sugeridas para reproduzir o ambiente do perfil.

- `esbenp.prettier-vscode` – Prettier (Formatador de código)
- `dbaeumer.vscode-eslint` – ESLint (Linting para JS/TS)
- `ms-python.python` – Suporte ao Python
- `ms-python.vscode-pylance` – IntelliSense para Python
- `ms-toolsai.jupyter` – Suporte a notebooks
- `eamodio.gitlens` – GitLens (Melhoria no Git)
- `PKief.material-icon-theme` – Ícones de arquivos
- `bradlc.vscode-tailwindcss` – Suporte ao Tailwind CSS
- `xabikos.JavaScriptSnippets` – Snippets úteis para JS

---

## 🧩 Configurações

Estas são as principais opções definidas no perfil:

```jsonc
{
  "editor.formatOnSave": true,
  "editor.tabSize": 2,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "eslint.format.enable": true,
  "python.formatting.provider": "black",
  "python.sortImports.args": ["--profile", "black"],
  "files.trimTrailingWhitespace": true,
  "files.insertFinalNewline": true,
  "files.autoSave": "afterDelay",
  "files.exclude": {
    "**/__pycache__": true,
    "**/*.pyc": true
  },
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Default Dark Modern"
}
```

💻 Requisitos

Para aproveitar ao máximo esta configuração, instale os seguintes pacotes globalmente (ou no ambiente virtual):

```bash
npm install -g prettier eslint
pip install black isort
```
