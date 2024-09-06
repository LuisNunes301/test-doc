# Documentação Engenharia de Dados
## Índice

1. [Introdução](#introdução)
2. [Objetivos](#objetivos)
3. [Programas, Frameworks e Bibliotecas Necessários](#programas-frameworks-e-bibliotecas-necessários)
   - [Ferramentas Requeridas na Máquina](#ferramentas-requeridas-na-máquina)
     - [Visual Studio Code](#visual-studio-code)
     - [Python](#python)
     - [Java e JDK](#java-e-jdk)
     - [Eclipse](#eclipse)
     - [Postman e Elastic](#postman-e-elastic)
     - [Git](#git)
4. [Comandos Necessários para Sobreviver](#comandos-necessários-para-sobreviver)
5. [Como Cortar Arquivos Rápido sem Modificar](#como-cortar-arquivos-rápido-sem-modificar)
6. [Qual Migrador Usar?](#qual-migrador-usar)
7. [Anotações no XTR Update](#anotações-no-xtr-update-ed-cura-op)
8. [O Que Colocar na Pasta de Operações](#o-que-colocar-na-pasta-de-operações)
9. [Envio Para o Diretório do Atualizador Padrão](#envio-para-o-diretório-do-atualizador-padrão)
10. [README](#readme)


## 1. Introdução

## 2. Objetivo
Fornecer um guia (quase)completo para configuração de ambiente, instalação de ferramentas e bibliotecas, além de instruções necessárias para a execução de tarefas de engenharia de dados, como manipulação de arquivos e utilização de migradores de dados.


## 3. Programas, Frameworks e Bibliotecas Necessários

### 3.1.Ferramentas Requeridas na Máquina

#### 3.1 Visual Studio Code
- **Extensões Necessárias:**
  - [Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-spring-boot)
  - [Extension Pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
  
- **Extensões Opcionais para Melhorar o Trabalho:**
  - [Rainbow CSV](https://marketplace.visualstudio.com/items?itemName=mechatroner.rainbow-csv)
  - [Excel Viewer](https://marketplace.visualstudio.com/items?itemName=GrapeCity.gc-excelviewer)

> **Observação:** Configurações visuais e pessoais do Visual Studio Code podem ser ajustadas de acordo com a preferência de cada pessoa.
#### 3.2 Python
- Instalar a última versão da linguagem de programação.
- **Recomendação:** Caso já tenha o Python instalado, execute:
```bash
    python --version  # Verifica a versão do Python instalada
    pip install --upgrade python  # Atualiza o Python
    pip install --upgrade pip  # Atualiza o pip
```
- **Dependências Necessárias:**
```bash
pip install openpyxl
pip install pandas
pip install beautifulsoup4
pip install requests
pip install ipykernel
pip install lxml
pip install selenium
```
#### 3.3 Java e JDK
- **Requisitos:**
    - [Java 8](https://www.java.com/pt-BR/download/ie_manual.jsp?locale=pt_BR)
    - [JDK Development Kit 17.0](https://download.oracle.com/java/17/archive/jdk-17.0.11_windows-x64_bin.msi)

#### 3.4 Eclipse
  -  Instalar a última versão do aplicativo: [Eclipse ide](https://www.eclipse.org/downloads/download.php?file=/oomph/epp/2024-06/R/eclipse-inst-jre-win64.exe)
  -  Adicionar o plugin no marketplace: [JSON Editor Plugin](https://marketplace.eclipse.org/).
#### 3.5 Postman e Elastic
- Configurar o Postman para testes de API.

#### 3.6 Git
- **Comandos Úteis:**
```bash
  git status # Verificar o status do repositório
  git add .  # Salvar atualizações na branch atual
  git commit -m "DESCRIÇÃO DA MODIFICAÇÃO"  # Realizar um commit com a descrição do nome da Entidade
  git checkout develop  # Entrar no diretório 'develop'
  git pull origin develop  # Verificar se há alguma atualização
  git merge <BRANCH_ATUALIZADA>  # Mesclar as alterações da branch atualizada para o repositório 'develop'
  git push origin develop  # Enviar o repositório atualizado para o GitLab
```
### 4. Comandos Necessários para Sobreviver
```bash
- `cd` - Mudar de diretório
- `rm` - Remover arquivos
- `sh -T arquivo` - Executar um script shell
- `ls` - Listar arquivos
```
### 5. Como Cortar Arquivos Rápido sem Modificar
 ```bash
    sed -n '1p; <inicio>,<fim>p' arquivo_original > arquivo_novo.csv
    awk 'NR>=10 && NR<=1000' x.csv > y.csv
```
### 6. Como Cortar Arquivos Rápido sem Modificar
- **Migrador-Docker:** Utilizado para arquivos `xlsx`.
- **Migrador-CSV:** Utilizado para arquivos `csv`.
- **Migrador-JSON:** Utilizado para arquivos `json`.
- **Migrador-API:** Utilizado para integrações de API.
- **Migrador-PNADCT:** Utilizado para dados específicos do PNADCT.
### 7. Anotações no XTR Update 

- **Qual # usar?**
  - `#Cura`: Curadoria
  - `#ED`: Engenharia de Dados
  - `#OP`: Operação

- **Template de Anotação:**
  - **Instrução de trabalho usada:** ED-000
  - **Necessário reoperar a carga:** SIM ou NÃO
  - **O que foi feito no app:** "Novo aplicativo", "Correção do mapping", "Correção do campo X", etc.


### 8. O Que Colocar na Pasta de Operações

- **Quando é migrador-docker:** Incluir todos os arquivos de configuração do Docker e scripts necessários para executar a migração.
- **Quando é CSV:** Colocar arquivos `.csv` originais e transformados, além de scripts de processamento de dados.
- **Quando é JSON:** Incluir arquivos `.json` originais, scripts de validação e transformação de dados.
- **Migrador API:** Colocar scripts de integração, configurações de conexão e documentação da API utilizada.

## 9. Envio Para o Diretório do Atualizador Padrão

Após a realização das etapas acima, acesse o terminal Git e, na raiz do projeto, versione sua contribuição. Utilize o fluxo de comandos Git mais frequente para essa finalidade:




## 10. README

Este documento é uma diretriz para os processos de Engenharia de Dados da empresa. Ele visa fornecer uma visão geral dos processos e procedimentos a serem seguidos pela equipe, garantindo a qualidade e a segurança dos dados coletados e processados.

Para contribuir com este documento, por favor, siga as seguintes etapas:

1. Leia o documento cuidadosamente e verifique se há alguma informação que precise ser atualizada ou corrigida.
2. Se você tiver alguma sugestão ou ideia para melhorar o documento, por favor, envie um e-mail para o gerente de Engenharia de Dados.
3. Se você precisar fazer alguma alteração no documento, por favor, faça um fork do repositório e envie um pull request com as alterações.

Agradecemos sua contribuição!