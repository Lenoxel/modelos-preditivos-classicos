# Modelos Preditivos Clássicos

[![Status do Projeto](https://img.shields.io/badge/status-Em%20Andamento-yellow)](https://shields.io/)

## 📝 Descrição

Este projeto tem como objetivo desenvolver as atividades e os projetos da disciplina de Modelos Preditivos Clássicos, parte da Pós-Graduação em Engenharia e Análise de Dados.

## 👥 Integrantes

- Bruno Venceslau Barbosa
- Carolina Queiroz de Sousa
- Gabriel Lenon Barros da Silva
- Gustavo Miguel Ferreira da Silva
- Pedro Henrique de Amaral lira

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.x
* **Bibliotecas Principais:** Pandas, Scikit-learn, Matplotlib, Seaborn
* **Ambiente de Desenvolvimento:** Google Colab
* **Controle de Versão:** Git & GitHub

## 🚀 Como Executar o Projeto

1.  Abra um notebook no Google Colab.
2.  Siga as instruções da seção **"Fluxo de Trabalho no Google Colab"** abaixo para configurar o ambiente e clonar o projeto.
3.  Instale as dependências executando a célula de código fornecida na seção de configuração.
4.  Abra a pasta `notebooks/` e execute os arquivos `.ipynb` da atividade ou projeto desejado.

## 📁 Estrutura de Pastas

```
/
├── notebooks/              # Contém os notebooks do Google Colab
├── requirements.txt        # Lista de dependências do projeto
└── README.md               # Este arquivo :)
```

---

## ✨ Nosso Fluxo de Trabalho no Google Colab (Passo a Passo)

Para manter nosso projeto organizado e evitar conflitos, vamos seguir este fluxo de trabalho **inteiramente dentro de células de código do Google Colab**.

> **Regra de Ouro:** NUNCA enviamos alterações diretamente para a branch `main`. Ela é o nosso código final e estável.

---

### **Etapa 0: ⚙️ Configuração Inicial (Só precisa fazer uma vez)**

Execute estas duas células no início do seu trabalho.

1.  **Monte seu Google Drive:** Isso conecta seu Colab ao seu Drive, permitindo salvar o projeto de forma permanente.
    ```python
    # Rode esta célula. Você precisará autorizar o acesso.
    from google.colab import drive
    drive.mount('/content/drive')
    ```

2.  **Clone o Repositório para o seu Drive:** Crie uma pasta `Colab_Projects` (ou o nome que preferir) no seu Google Drive e clone o projeto lá dentro.
    ```bash
    # Navega para a pasta desejada no seu Drive
    %cd /content/drive/MyDrive/Colab_Projects/

    # Clone o repositório (substitua pela URL do seu projeto)
    !git clone https://github.com/Lenoxel/modelos-preditivos-classicos.git
    ```
    *Da próxima vez que for trabalhar, você pode pular este passo e ir direto para a Etapa 1, apenas navegando para a pasta já existente com `%cd /content/drive/MyDrive/Colab_Projects/modelos-preditivos-classicos`.*

### **Etapa 1: 🔄 Sincronize e Crie sua Branch de Trabalho**

Antes de começar a codificar, sempre garanta que você tem a versão mais atual do projeto e crie uma branch separada para sua tarefa.

```bash
# Navega para a pasta do projeto que você clonou
%cd /content/drive/MyDrive/Colab_Projects/modelos-preditivos-classicos

# Garante que está na branch principal
!git checkout main

# Puxa as últimas atualizações do GitHub
!git pull origin main

# Agora, crie sua branch de trabalho (substitua com seu nome/tarefa)
# Exemplo: !git checkout -b maria/limpeza-de-dados
!git checkout -b seu-nome/objetivo-da-tarefa
```

### **Etapa 2: 💻 Trabalhe no Projeto**

Agora sim! Use a interface do Google Drive para navegar até a pasta do projeto e abrir o notebook em que você precisa trabalhar. Faça suas alterações, crie seus códigos e **lembre-se de salvar o notebook (Ctrl + S)**.

### **Etapa 3: 🚀 Envie suas Alterações para o GitHub**

Quando terminar uma parte do trabalho ou ao final do dia, salve seu progresso no Git.

1.  **Configure suas credenciais do Git (só precisa fazer na primeira vez que for enviar):**
    ```bash
    !git config --global user.name "Seu Nome Completo"
    !git config --global user.email "seu-email-de-cadastro@github.com"
    ```

2.  **Adicione e envie suas alterações:**
    ```bash
    # Navega de volta para a pasta do projeto, caso tenha saído
    %cd /content/drive/MyDrive/Colab_Projects/modelos-preditivos-classicos

    # 1. Adiciona TODOS os arquivos que você modificou
    !git add .

    # 2. Cria um "commit" (uma foto do seu progresso) com uma mensagem clara
    # Exemplo: !git commit -m "feat: Adiciona tratamento para valores nulos na coluna idade"
    !git commit -m "tipo: O que você fez de forma resumida"

    # 3. Envia o commit para a SUA branch no GitHub
    # Exemplo: !git push origin maria/limpeza-de-dados
    !git push origin seu-nome/objetivo-da-tarefa
    ```
    *O Colab/Git pode pedir sua autenticação do GitHub. A forma mais fácil é usar um [Token de Acesso Pessoal](https://docs.github.com/pt/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) como senha.*

### **Etapa 4: ✅ Abra um Pull Request (PR) e Faça o Merge**

1.  **Vá para o site do GitHub:** Abra a página do nosso repositório.
2.  **Crie o Pull Request:** O GitHub vai mostrar um aviso em amarelo para você criar um **Pull Request** da sua branch. Clique no botão.
3.  **Descreva e Revise:** Dê um título claro, descreva o que você fez e marque os colegas como "reviewers".
4.  **Merge:** Após a revisão e aprovação, o código pode ser integrado à branch `main` clicando no botão "Merge pull request".

**Pronto!** Sua contribuição agora está na versão oficial do projeto. Para a próxima tarefa, comece novamente pela **Etapa 1**.