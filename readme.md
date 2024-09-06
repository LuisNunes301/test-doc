# Documentação Engenharia de Dados
## Índice

1. [Introdução](#1-introdução)
2. [Objetivos](#2-objetivos)
3. [Programas, Frameworks e Bibliotecas Necessários](#3-programas-frameworks-e-bibliotecas-necessários)
   - [Ferramentas Requeridas na Máquina](#31-ferramentas-requeridas-na-máquina)
     - [Visual Studio Code](#311-visual-studio-code)
     - [Python](#312-python)
     - [Java e JDK](#313-java-e-jdk)
     - [Eclipse](#314-eclipse)
     - [Postman e Elastic](#315-postman-e-elastic)
     - [Git](#316-git)
4. [Comandos Necessários para Sobreviver](#4-comandos-necessários-para-sobreviver)
5. [Como Cortar Arquivos Rápido sem Modificar](#5-como-cortar-arquivos-rápido-sem-modificar)
6. [Qual Migrador Usar?](#6-qual-migrador-usar)
7. [Anotações no XTR Update (ED - CURA - OP)](#7-anotações-no-xtr-update-ed---cura---op)
8. [O Que Colocar na Pasta de Operações](#8-o-que-colocar-na-pasta-de-operações)
9. [Envio Para o Diretório do Atualizador Padrão](#9-envio-para-o-diretório-do-atualizador-padrão)
10. [README](#10-readme)


## 1. Introdução

## 2. Objetivos
Fornecer um guia (quase)completo para configuração de ambiente, instalação de ferramentas e bibliotecas, além de instruções necessárias para a execução de tarefas de engenharia de dados, como manipulação de arquivos e utilização de migradores de dados.


## 3. Programas, Frameworks e Bibliotecas Necessários

### 3.1. Ferramentas Requeridas na Máquina

##### 3.1.1 Visual Studio Code
- **Extensões Necessárias:**
  - [Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-spring-boot)
  - [Extension Pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
  
- **Extensões Opcionais para Melhorar o Trabalho:**
  - [Rainbow CSV](https://marketplace.visualstudio.com/items?itemName=mechatroner.rainbow-csv)
  - [Excel Viewer](https://marketplace.visualstudio.com/items?itemName=GrapeCity.gc-excelviewer)

> **Observação:** Configurações visuais e pessoais do Visual Studio Code podem ser ajustadas de acordo com a preferência de cada pessoa.
##### 3.1.2 Python
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
##### 3.1.3 Java e JDK
- **Requisitos:**
    - [Java 8](https://www.java.com/pt-BR/download/ie_manual.jsp?locale=pt_BR)
    - [JDK Development Kit 17.0](https://download.oracle.com/java/17/archive/jdk-17.0.11_windows-x64_bin.msi)

##### 3.1.4 Eclipse
  -  Instalar a última versão do aplicativo: 
      - [Eclipse ide](https://www.eclipse.org/downloads/download.php?file=/oomph/epp/2024-06/R/eclipse-inst-jre-win64.exe)
  -  Adicionar o plugin no marketplace: 
      - [JSON Editor Plugin](https://marketplace.eclipse.org/).
##### 3.1.5 Postman e Elastic
- Configurar o Postman para testes de API.

##### 3.1.6 Git
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
  - O comando usado `awk` para selecionar as linhas de 10 a 1000 do arquivo x.csv e salva essas linhas no arquivo y.csv.
  - O comando `sed` -n '1p; <inicio>,<fim>p' arquivo_original > arquivo_novo.csv copia a primeira linha e o intervalo de linhas entre <inicio> e <fim> do arquivo arquivo_original para arquivo_novo.csv.
  Este comando é útil para manter o cabeçalho de um arquivo CSV ao selecionar um subconjunto de linhas.
### 6. Qual Migrador Usar?
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
>**Observação** Copiar e colar, com ctrl + shift + v para que cole sem formatação.


### 8. O Que Colocar na Pasta de Operações

- **Quando é migrador-docker:** Incluir todos os arquivos de configuração do Docker e scripts necessários para executar a migração.
- **Quando é CSV:** Colocar arquivos `.csv` originais e transformados, além de scripts de processamento de dados.
- **Quando é JSON:** Incluir arquivos `.json` originais, scripts de validação e transformação de dados.
- **Migrador API:** Colocar scripts de integração, configurações de conexão e documentação da API utilizada.

## 9. Envio Para o Diretório da Operação

Após a realização das etapas acima, acesse o terminal Git e, na raiz do projeto, versione sua contribuição. Utilize o fluxo de comandos Git mais frequente para essa finalidade:




## 10. README

Este documento é uma diretriz para os processos de Engenharia de Dados da empresa. Ele visa fornecer uma visão geral dos processos e procedimentos a serem seguidos pela equipe, garantindo a qualidade e a segurança dos dados coletados e processados.

Para contribuir com este documento, por favor, siga as seguintes etapas:

1. Leia o documento cuidadosamente e verifique se há alguma informação que precise ser atualizada ou corrigida.
2. Se você tiver alguma sugestão ou ideia para melhorar o documento, por favor, envie um e-mail para o gerente de Engenharia de Dados.
3. Se você precisar fazer alguma alteração no documento, por favor, faça um fork do repositório e envie um pull request com as alterações.

Agradecemos sua contribuição!