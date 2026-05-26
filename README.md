# aulas-praticas-de-linux-da-certifica-çao-google-cybersecurity
Guia de Comandos Básicos do Linux (Navegação e Leitura de Arquivos)
# 🐧 Guia de Comandos Básicos do Linux (Navegação e Leitura de Arquivos)

Este repositório contém o passo a passo e a explicação dos comandos Linux utilizados para navegar pelo sistema de arquivos, listar conteúdos e ler dados de arquivos de texto.

---

## 📋 Sumário
1. [Task 1: Verificar Diretório Atual e Listar Conteúdo](#task-1-verificar-diretório-atual-e-listar-conteúdo)
2. [Task 2: Mudar de Diretório (Caminhos Absolutos vs. Relativos)](#task-2-mudar-de-diretório-caminhos-absolutos-vs-relativos)
3. [Task 3: Localizar e Ler o Conteúdo de um Arquivo](#task-3-localizar-e-ler-o-conteúdo-de-um-arquivo)
4. [Task 4: Exibir as Primeiras Linhas de um Arquivo](#task-4-exibir-as-primeiras-linhas-de-um-arquivo)
5. [🧠 Resumo dos Comandos Aprendidos](#-resumo-dos-comandos-aprendidos)

---

## Task 1: Verificar Diretório Atual e Listar Conteúdo

Nesta etapa, validamos em qual pasta do sistema estávamos trabalhando e o que havia dentro dela.

* **Exibir o diretório de trabalho atual:**
    ```bash
    pwd
    ```
    *Output esperado:* `/home/analyst` (Diretório home do usuário).

* **Listar os arquivos e pastas do diretório atual:**
    ```bash
    ls
    ```
    *Output esperado:* `logs  projects  reports  temp`

---

## Task 2: Mudar de Diretório (Caminhos Absolutos vs. Relativos)

Navegamos para a pasta `reports` utilizando duas abordagens diferentes de caminhos.

* **Opção A: Usando caminho relativo** (parte de onde você está agora):
    ```bash
    cd reports
    ```
* **Opção B: Usando caminho absoluto** (inicia da raiz `/` do sistema):
    ```bash
    cd /home/analyst/reports
    ```

Ao listar o conteúdo com `ls`, descobrimos a subpasta:
* 📁 **Subpasta encontrada:** `users`

---

## Task 3: Localizar e Ler o Conteúdo de um Arquivo

Navegamos até o destino final para inspecionar os dados de um arquivo específico.

* **Navegar até a pasta final:**
    ```bash
    cd /home/analyst/reports/users
    ```
* **Ler o conteúdo do arquivo `Q1_added_users.txt`:**
    ```bash
    cat Q1_added_users.txt
    ```

> 💡 **Nota:** O comando `cat` imprime todo o conteúdo do arquivo na tela.


---

## Task 4: Exibir as Primeiras Linhas de um Arquivo

Para arquivos grandes, como logs de servidor, nem sempre queremos ver o arquivo inteiro. Usamos uma ferramenta para limitar a saída.

* **Navegar até a pasta de logs:**
    ```bash
    cd /home/analyst/logs
    ```
* **Exibir as 10 primeiras linhas do arquivo `server_logs.txt`:**
    ```bash
    head server_logs.txt
    ```

> 📌 **Análise de Log:** Nas 10 primeiras linhas exibidas pelo comando `head`, identificamos o total de **3 mensagens de aviso (warnings)**.

---

## 🧠 Resumo dos Comandos Aprendidos

| Comando | Descrição | Exemplo de Uso |
| :--- | :--- | :--- |
| **`pwd`** | *Print Working Directory* - Mostra a pasta onde você está agora. | `pwd` |
| **`ls`** | *List* - Lista os arquivos e pastas do diretório atual. | `ls` |
| **`cd`** | *Change Directory* - Muda de pasta (navegação). | `cd /home/analyst` |
| **`cat`** | *Concatenate* - Exibe o conteúdo completo de um arquivo de texto. | `cat arquivo.txt` |
| **`head`** | Exibe as linhas iniciais de um arquivo (padrão: 10 linhas). | `head log.txt` |
<img width="868" height="568" alt="linux" src="https://github.com/user-attachments/assets/b36448ca-1d4c-4636-b9a0-8049f5772a4e" />
<img width="864" height="564" alt="image" src="https://github.com/user-attachments/assets/c1aa804a-3b7f-4c52-95f1-3894af5442d7" />
<img width="869" height="565" alt="image" src="https://github.com/user-attachments/assets/e5946c1c-1b28-436a-8d8f-e636d80c4d4c" />






