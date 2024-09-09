![enter image description here](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)![enter image description here](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)![enter image description here](https://img.shields.io/badge/Eclipse-2C2255?style=for-the-badge&logo=eclipse&logoColor=white)![enter image description here](https://img.shields.io/badge/Elastic_Search-005571?style=for-the-badge&logo=elasticsearch&logoColor=whit)![enter image description here](https://img.shields.io/badge/GitLab-330F63?style=for-the-badge&logo=gitlab&logoColor=white)
# Documentação Engenharia de Dados
## Índice

1. [Introdução.](#1-introdução)
2. [Objetivos.](#2-objetivos)
3. [Programas, Frameworks e Bibliotecas Necessários.](#3-programas-frameworks-e-bibliotecas-necessários)
   - [Ferramentas Requeridas na Máquina.](#31-ferramentas-requeridas-na-máquina)
     - [Visual Studio Code](#311-visual-studio-code)
     - [Python](#312-python)
     - [Java e JDK](#313-java-e-jdk)
     - [Eclipse](#314-eclipse)
     - [Postman e Elastic](#315-postman-e-elastic)
     - [Git](#316-git)
4. [Comandos Necessários para Sobreviver.](#4-comandos-necessários-para-sobreviver)
5. [Como Cortar Arquivos Rápido sem Modificar.](#5-como-cortar-arquivos-rápido-sem-modificar)
6. [Qual Migrador Usar?](#6-qual-migrador-usar)
7. [Anotações no XTR Update.](#7-anotações-no-xtr-update)
8. [O Que Colocar na Pasta de Operações.](#8-o-que-colocar-na-pasta-de-operações)
9. [Rotina de versionamento de codigo.](#9-rotina-de-versionamento-de-codigo)
10. [Confie em nós.](#10-confie-em-nós)


## 1. Introdução.
Bem-vindo ao guia de **Engenharia de Dados**!

Este documento é uma **diretriz** para os processos de **Engenharia de Dados** da Consiste, visando fornecer uma visão geral dos processos e procedimentos a serem seguidos pela equipe, garantindo a **qualidade** e a **segurança** dos dados coletados e processados.

Este guia é dividido em seções, cada uma abordando um tópico específico, desde a **apresentação** até a **configuração de recursos** e procedimentos para a **realização de atividades**.

Aqui, você encontrará informações sobre como **preparar o ambiente de trabalho**, **instalar utilitários e bibliotecas essenciais**, além de instruções para a **execução de tarefas de engenharia de dados**, como **gerenciamento de arquivos** e utilização de **migradores de dados**.



- **Índice**: fornece uma visão geral do conteúdo do guia.
- **Introdução**: apresenta o objetivo e o escopo do guia.
- **Objetivos**: descreve os objetivos do guia.
- **Programas, Frameworks e Bibliotecas Necessários**: lista as ferramentas e bibliotecas necessárias para a execução de tarefas de engenharia de dados.
- **Comandos Necessários para Sobreviver**: fornece comandos úteis para a execução de tarefas de engenharia de dados.
- **Como Cortar Arquivos Rápido sem Modificar**: fornece instruções para cortar arquivos rapidamente sem modificar.
- **Qual Migrador Usar?**: descreve os diferentes tipos de migradores e quando usá-los.
- **Anotações no XTR Update**: fornece instruções para anotar no XTR Update.
- **O Que Colocar na Pasta de Operações**: descreve o que colocar na pasta de operações.
- **Comandos necessarios para upar um repositório para o GitLab**: fornece comandos necessários para upar um repositório para o GitLab.
- **README**: fornece informações sobre como contribuir com o guia.

Esperamos que este guia seja útil para você! Se tiver alguma dúvida ou precisar de mais ajuda, sinta-se à vontade para perguntar.
## 2. Objetivos.
Fornecer um guia (quase)completo para configuração de ambiente, instalação de ferramentas e bibliotecas, além de instruções necessárias para a execução de tarefas de engenharia de dados, como manipulação de arquivos e utilização de migradores de dados.


## 3. Programas, Frameworks e Bibliotecas Necessários.

### 3.1. Ferramentas Requeridas na Máquina.

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
    - [JDK Development Kit 17.0](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)

##### 3.1.4 Eclipse
  -  Instalar a última versão do aplicativo: 
      - [Eclipse ide](https://eclipseide.org)
  -  Adicionar o plugin no marketplace: 
      - [JSON Editor Plugin](https://marketplace.eclipse.org/content/json-editor-plugin).
##### 3.1.5 Postman e Elastic
- [Postman](https://www.postman.com/downloads/)
- Configurar o Postman para testes de API.
- Sandbox: http://sandbox.consiste.com.br:5601/app/dev_tools#/console
>**Observação:** Precisa estar com a VPN ligada para acessar.

##### 3.1.6 Git
  - Instalar [git](https://git-scm.com/download/)
##### 3.1.7 Notepad++
- Instalar [Notepad++](https://notepad-plus-plus.org/downloads/)
##### 3.1.8 Emditor
- Instalar [Emditor](https://www.emeditor.com/#download)
### 4. Comandos Necessários para Sobreviver.
```bash
- `cd` - Mudar de diretório
- `rm` - Remover arquivos
- `sh -T arquivo` - Executar um script shell
- `ls` - Listar arquivos do diretorio corrente
- `cat arquivo` - Exibe conteudo de um arquivo
```
### 5. Como Cortar Arquivos Rápido sem Modificar.
 ```bash
    sed -n '1p; <inicio>,<fim>p' x > y
    ou
    awk 'NR>=10 && NR<=1000' x.csv > y.csv
  
```  
  - O comando usado `awk` para selecionar as linhas de 10 a 1000 do arquivo x.csv e salva essas linhas no arquivo y.csv.
  - O comando `sed` -n '1p; <inicio>,<fim>p' arquivo_original > arquivo_novo.csv copia a primeira linha e o intervalo de linhas entre <inicio> e <fim> do arquivo arquivo_original para arquivo_novo.csv.
  Este comando é útil para manter o cabeçalho de um arquivo CSV ao selecionar um subconjunto de linhas.
### 6. Qual Migrador Usar?
- **Migrador-Docker:** Utilizar quando for necessario normalizar para quando o tipo de arquivo for diferente de `csv`.
- **Migrador-CSV:** Utilizado para arquivos `csv`.
- **Migrador-JSON:** Utilizado para arquivos `json`.
- **Migrador-API:** Utilizado para integrações de API.
- **Migrador-PNADCT:** Utilizado para dados específicos do PNADCT.
### 7. Anotações no XTR Update.

- **Qual # usar?**
  - `#Cura`: Curadoria
  - `#ED`: Engenharia de Dados
  - `#OP`: Operação
    - 001 Migrador-CSV
    - 002 Migrador-API
    - 004 Migrador-Docker
    - 006 Migrador-Json
- **Template de Anotação:**
  - **Instrução de trabalho usada:** XX-00X (mudar correspondente a anotação).
  - **Necessário reoperar a carga:** SIM ou NÃO
  - **O que foi feito no app:** "Novo aplicativo", "Correção do mapping", "Correção do campo X", etc.
>**Observação** Copiar e colar, com ctrl + shift + v para que cole sem formatação.

### 8. O Que Colocar na Pasta de Operações.
**Verificar e não subir os `logs` e arquivos que estão no `/dataNormalizadorAssets`**
- **Quando é migrador-docker:** Incluir todos os arquivos na pasta da operacão, seguindo o seguinte modelo.
![docker](/assets/docker.png)

- **Quando é Migrador-CSV:** Incluir todos os arquivos na pasta da operacão, seguindo o seguinte modelo.
![csv](/assets/csv.png)

>**Se atentar para quando o arquivo a ser executado tiver mais de 1M docs, a entidade deve seguir o seguinte modelo na pasta da operações.**
![csv-ingestor](/assets/csv-ingestor.png)
- **Quando é JSON:** Incluir todos os arquivos na pasta da operacão, seguindo o seguinte modelo, há de reparar que é bem semelhante ao **Migrador-CSV**.
![json](/assets/json.png)

- **Migrador API:** Incluir todos os arquivos na pasta da operacão, seguindo o seguinte modelo, há de reparar que é bem semelhante ao **Migrador-CSV**.
![api](/assets/api.png)

## 9. Rotina de versionamento de codigo.

```bash
  git status # Verificar o status do repositório
  git add .  # Salvar atualizações na branch atual
  git commit -m "DESCRIÇÃO DA MODIFICAÇÃO"  # Realizar um commit com a descrição do nome da Entidade
  git checkout develop  # Entrar no diretório 'develop'
  git pull origin develop  # Verificar se há alguma atualização
  git merge <BRANCH_ATUALIZADA>  # Mesclar as alterações da branch atualizada para o repositório 'develop'
  git push origin develop  # Enviar o repositório atualizado para o GitLab
```



## 10. Confie em nós.

Este documento é uma diretriz para os processos de Engenharia de Dados da Consiste. Ele visa fornecer uma visão geral dos processos e procedimentos a serem seguidos pela equipe, garantindo a qualidade e a segurança dos dados coletados e processados.

Para contribuir com este documento, por favor, siga as seguintes etapas:

1. Leia o documento cuidadosamente e verifique se há alguma informação que precise ser atualizada ou corrigida.
2. Se você tiver alguma sugestão ou ideia para melhorar o documento, por favor, envie um e-mail para o coordenador da Engenharia de Dados.
3. Se você precisar fazer alguma alteração no documento, por favor, faça um fork do repositório e envie um pull request com as alterações.

Agradecemos sua contribuição!