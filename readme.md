# Documentação Engenharia de Dados

### Objetivo
Fornecer um guia (quase)completo para configuração de ambiente, instalação de ferramentas e bibliotecas, além de instruções necessárias para a execução de tarefas de engenharia de dados, como manipulação de arquivos e utilização de migradores de dados.

## Programas, Frameworks e Bibliotecas Necessários

### 1. Ferramentas Requeridas na Máquina

#### 1.1 Visual Studio Code
- **Extensões Necessárias:**
  - [Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-spring-boot)
  - [Extension Pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
  
- **Extensões Opcionais para Melhorar o Trabalho:**
  - [Rainbow CSV](https://marketplace.visualstudio.com/items?itemName=mechatroner.rainbow-csv)
  - [Excel Viewer](https://marketplace.visualstudio.com/items?itemName=GrapeCity.gc-excelviewer)

> **Observação:** Configurações visuais e pessoais do Visual Studio Code podem ser ajustadas de acordo com a preferência de cada pessoa.
#### 1.2 Python
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
#### 1.3 Java e JDK
- **Requisitos:**
  - Java 8
  - JDK Development Kit 17.0

#### 1.4 Eclipse
- Instalar a última versão do aplicativo.
- Adicionar o plugin no marketplace: [JSON Editor Plugin](https://marketplace.eclipse.org/).
#### 1.5 Postman e Elastic
- Configurar o Postman para testes de API.

#### 1.6 Git
- **Comandos Úteis:**
```bash
  git add .  # Salvar atualizações na branch atual
  git commit -m "DESCRIÇÃO DA MODIFICAÇÃO"  # Realizar um commit com a descrição do nome da Entidade
  git checkout develop  # Entrar no diretório 'develop'
  git pull origin develop  # Verificar se há alguma atualização
  git merge <BRANCH_ATUALIZADA>  # Mesclar as alterações da branch atualizada para o repositório 'develop'
  git push origin develop  # Enviar o repositório atualizado para o GitLab
```
### 2. Comandos Necessários para Sobreviver
```bash
- `cd` - Mudar de diretório
- `rm` - Remover arquivos
- `sh -T arquivo` - Executar um script shell
- `ls` - Listar arquivos
```
### 3. Como Cortar Arquivos Rápido sem Modificar
 ```bash
    sed -n '1p; <inicio>,<fim>p' arquivo_original > arquivo_novo.csv
    awk 'NR>=10 && NR<=1000' x.csv > y.csv
```
### 4. Como Cortar Arquivos Rápido sem Modificar
- **Migrador-Docker:** Utilizado para arquivos `xlsx`.
- **Migrador-CSV:** Utilizado para arquivos `csv`.
- **Migrador-JSON:** Utilizado para arquivos `json`.
- **Migrador-API:** Utilizado para integrações de API.
- **Migrador-PNADCT:** Utilizado para dados específicos do PNADCT.
7anotacoes no xtr update (ED - CURA - OP)
    
    7.1 Qual # usar? 
        7.1.1 #Cura
            texto dizendo quando usar
        7.1.2 #ED
            texto dizendo quando usar
        7.1.3 #OP
            texto dizendo quando usar

    7.2 Template
        Instrução de trabalho usada: ED-000
        Necessário reoperar a carga: SIM ou NÃO
        O que foi feito no app: "Novo aplicativo" ou "Correção do mapping", "correção do campo X".

8quais coisas botar na pasta oparacoes
    8.1 quando é migrador-docker
    8.2 quando é csv
    8.3 quando é json
    8.4 migrador api
9   Envio Para o Diretório do Atualizador Padrão
Após a realização das etapas acima, acesse seu terminal git e, na raiz do projeto, versione sua contribuição. Segue o fluxo de comandos git mais frequente para essa finalidade:


# Indice 

1. [Introdução](#introdução)
2. [Objetivos](#objetivos)
3. [Escopo](#escopo)
4. [Processos de Engenharia de Dados](#processos-de-engenharia-de-dados)
    1. [Coleta de Dados](#coleta-de-dados)
    2. [Processamento de Dados](#processamento-de-dados)
    3. [Armazenamento de Dados](#armazenamento-de-dados)
    4. [Análise de Dados](#análise-de-dados)
    5. [Visualização de Dados](#visualização-de-dados)
5. [Responsabilidades](#responsabilidades)
6. [Controle de Versão](#controle-de-versão)

## Introdução

Este documento tem como objetivo descrever os processos de Engenharia de Dados utilizados pela empresa, garantindo a qualidade e a segurança dos dados coletados e processados.

## Objetivos

* Definir os processos de Engenharia de Dados a serem seguidos pela equipe;
* Garantir a qualidade e a segurança dos dados coletados e processados;
* Fornecer diretrizes para a coleta, processamento, armazenamento, análise e visualização de dados.

## Escopo

Este documento se aplica a todos os colaboradores da empresa que trabalham com Engenharia de Dados.

## Processos de Engenharia de Dados

### Coleta de Dados

* Definição dos requisitos de coleta de dados;
* Seleção das fontes de dados;
* Coleta de dados utilizando ferramentas e técnicas adequadas.

### Processamento de Dados

* Limpeza e transformação de dados;
* Validação e verificação de dados;
* Processamento de dados utilizando ferramentas e técnicas adequadas.

### Armazenamento de Dados

* Definição da estrutura de armazenamento de dados;
* Seleção da tecnologia de armazenamento de dados;
* Armazenamento de dados de forma segura e eficiente.

### Análise de Dados

* Definição dos objetivos de análise de dados;
* Seleção das técnicas e ferramentas de análise de dados;
* Análise de dados para extrair insights e conhecimentos.

### Visualização de Dados

* Definição dos objetivos de visualização de dados;
* Seleção das ferramentas e técnicas de visualização de dados;
* Visualização de dados para comunicar insights e conhecimentos.

## Responsabilidades

* O gerente de Engenharia de Dados é responsável por garantir a implementação e manutenção dos processos de Engenharia de Dados;
* Os colaboradores de Engenharia de Dados são responsáveis por seguir os processos de Engenharia de Dados definidos.

## Controle de Versão

Este documento será revisado e atualizado anualmente, ou sempre que necessário.

## README

Este documento é uma diretriz para os processos de Engenharia de Dados da empresa. Ele visa fornecer uma visão geral dos processos e procedimentos a serem seguidos pela equipe, garantindo a qualidade e a segurança dos dados coletados e processados.

Para contribuir com este documento, por favor, siga as seguintes etapas:

1. Leia o documento cuidadosamente e verifique se há alguma informação que precise ser atualizada ou corrigida.
2. Se você tiver alguma sugestão ou ideia para melhorar o documento, por favor, envie um e-mail para o gerente de Engenharia de Dados.
3. Se você precisar fazer alguma alteração no documento, por favor, faça um fork do repositório e envie um pull request com as alterações.

Agradecemos sua contribuição!