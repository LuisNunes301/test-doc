![enter image description here](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)![enter image description here](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)![enter image description here](https://img.shields.io/badge/Eclipse-2C2255?style=for-the-badge&logo=eclipse&logoColor=white)![enter image description here](https://img.shields.io/badge/Elastic_Search-005571?style=for-the-badge&logo=elasticsearch&logoColor=whit)![enter image description here](https://img.shields.io/badge/GitLab-330F63?style=for-the-badge&logo=gitlab&logoColor=white)


# Documentação Engenharia de Dados
## Índice

1. [Introdução.][def]
2. [Objetivos.][def2]
3. [Programas, Frameworks e Bibliotecas Necessários.][def3]  
   - 3.1 [Ferramentas Requeridas na Máquina.][def4]  
      - 3.1.1 [Visual Studio Code][def5]  
      3.1.2 [Python][def6]  
      3.1.3 [Java e JDK][def7]  
      3.1.4 [Eclipse][def8]  
      3.1.5 [Postman e Elastic][def9]  
      3.1.6 [Git][def10]  
      3.1.7 [Notepad++][def11]  
      3.1.8 [Emditor][def12]
4. [Comandos Necessários para Sobreviver.][def13]
5. [Como Cortar Arquivos Rápido sem Modificar.][def14]
6. [Qual Migrador Usar?][def15]
7. [Anotações no XTR Update.][def16]
8. [O Que Colocar na Pasta de Operações.][def17]
9. [Rotina de versionamento de codigo.][def18]
10. [Codigos para a verifição da migração dos dados.][def19]
11. [Funcionamento do Docker][def20]
12. [Casos do DIA-DIA][def21]
13. [Faça parte da nossa equipe, contribua para o nosso crescimento.][def22]


## 1. Introdução.


Bem-vindo ao guia de **Engenharia de Dados**!

Este documento é uma **diretriz** para os processos de **Engenharia de Dados** da Consiste, visando fornecer uma visão geral dos processos e procedimentos a serem seguidos pela equipe, garantindo a **qualidade** e a **segurança** dos dados coletados e processados.

Este guia é dividido em seções, cada uma abordando um tópico específico, desde a **apresentação** até a **configuração de recursos** e procedimentos para a **realização de atividades**.

Aqui, você encontrará informações sobre como **preparar o ambiente de trabalho**, **instalar utilitários e bibliotecas essenciais**, além de instruções para a **execução de tarefas de engenharia de dados**, como **gerenciamento de arquivos** e utilização de **migradores de dados**.

### Estrutura do Guia:

- **Objetivos**: Apresenta os principais objetivos deste guia, destacando as metas que você deve alcançar ao seguir estas diretrizes.
  
- **Programas, Frameworks e Bibliotecas Necessários**: Detalha as ferramentas, frameworks e bibliotecas que devem ser instaladas e configuradas em sua máquina para garantir um ambiente de trabalho adequado.

- **Comandos Necessários para Sobreviver**: Uma lista de comandos essenciais que irão facilitar a execução de diversas tarefas no ambiente de Engenharia de Dados.

- **Como Cortar Arquivos Rápido sem Modificar**: Aborda técnicas para cortar arquivos de forma eficiente, sem modificar seu conteúdo original.

- **Qual Migrador Usar?**: Fornece orientações sobre a escolha de migradores de dados, explicando qual utilizar para cada situação.

- **Anotações no XTR Update**: Explica como fazer anotações adequadas no sistema XTR Update para rastrear atualizações e mudanças.

- **O Que Colocar na Pasta de Operações**: Lista os itens essenciais que devem ser armazenados na pasta de operações do projeto para garantir uma boa organização.

- **Rotina de Versionamento de Código**: Aborda as melhores práticas para versionamento de código, garantindo a rastreabilidade e controle de versões.

- **Códigos para a Verificação da Migração dos Dados**: Oferece trechos de código e técnicas para verificar a migração de dados de forma eficiente e segura.

- **Funcionamento do Docker**: Apresenta uma visão geral sobre como o Docker funciona e como ele pode ser utilizado no ambiente de Engenharia de Dados, além de resolução de um problema do dia a dia.

- **Faça parte da nossa equipe, contribua para o nosso crescimento**: Finaliza com uma mensagem de confiança nas práticas e processos descritos no guia.

Esperamos que este guia seja útil para você! Se tiver alguma dúvida ou precisar de mais ajuda, sinta-se à vontade para perguntar.
## 2. Objetivos.
Fornecer um guia (quase) completo para configuração de ambiente, instalação de ferramentas e bibliotecas, além de instruções necessárias para a execução de tarefas de engenharia de dados, como manipulação de arquivos e utilização de migradores de dados.


## 3. Programas, Frameworks e Bibliotecas Necessários.

### 3.1. Ferramentas Requeridas na Máquina.

##### 3.1.1 Visual Studio Code
- Instalar [Vscode](https://code.visualstudio.com/Download)
- **Extensões Necessárias:**
  - [Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-spring-boot)
  - [Extension Pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
  
- **Extensões Opcionais para Melhorar o Trabalho:**
  - [Rainbow CSV](https://marketplace.visualstudio.com/items?itemName=mechatroner.rainbow-csv)
  - [Excel Viewer](https://marketplace.visualstudio.com/items?itemName=GrapeCity.gc-excelviewer)

> **Observação:** As configurações visuais e personalizadas do Visual Studio Code podem ser ajustadas de acordo com as preferências individuais de cada usuário..
##### 3.1.2 Python
- Instalar [Python](https://www.python.org/downloads/)
- Instalar a última versão da linguagem de programação.
- **Recomendação:** Caso já tenha o Python instalado, execute:
```bash
    python --version  # Verifica a versão do Python instalada
    pip install --upgrade python  # Atualiza o Python
    pip install --upgrade pip  # Atualiza o pip
```
- **Dependências Necessárias:**
```bash
pip install openpyxl pandas beautifulsoup4 requests ipykernel lxml selenium
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
- `file --mime-encoding` NOMEARQUIVO.csv
```
### 5. Como Cortar Arquivos Rápido sem Modificar.
 ```bash
    sed -n '1p; <inicio>,<fim>p' x > y
    ou
    awk 'NR == 1|| NR>=10 && NR<=1000' x.csv > y.csv
  
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
- **Template de Anotação para OP:**
  - **Instrução de trabalho usada:** XX-00X (mudar correspondente a anotação).
  - **Necessário reoperar a carga:** SIM ou NÃO
  - **O que foi feito no app:** "Novo aplicativo", "Correção do mapping", "Correção do campo X", etc.
>**Observação** Copiar e colar, com ctrl + shift + v para colar sem formatação.

### 8. O Que Colocar na Pasta de Operações.
**Verificar e não subir os `logs` e arquivos que estão no `/dataNormalizadorAssets`**

- **Quando é migrador-docker:** Incluir todos os arquivos na pasta da operacão, seguindo o seguinte modelo.
![docker](/assets/docker.png)
> Observação .jar é pacote que contém arquivos relacionados a um projeto Java, como codigo compilado, bibliotecas, metadados e recursos. Deve ser gerado pela IDE ou por linha de comando.
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
  git pull # Verificar se há alguma atualização
  git push # Enviar o repositório atualizado para o GitLab
```

## 10. Codigos para a verifição da migração dos dados.
**Uma breve rotina de codigo utilizado no elastic search.**
> Precisa estar com a VPN ligada
##### Comandos Básicos

```bash
GET e434_c5/_mapping

```
>Nota: Este comando obtém a estrutura do índice (_mapping).
```bash
e434_c5/_count
``` 
>Nota: Este comando conta o número de documentos no índice.
```bash
GET e434_c5/_search
``` 
>Nota: Este comando realiza uma busca geral no índice.

```plaintext
GET e434_c5/_search
{
  "query": {
    "match": {
      "FIELD": "TEXT"
    }
  }
}
```
>Nota: Faz uma busca onde o campo "FIELD" contém "TEXT".
```
DELETE e434_c5 
```
>Nota: Este comando exclui o índice e434_c5, removendo todos os dados.


Para se aprofundar mais no uso do Elasticsearch, recomendo consultar a [documentação oficial do Elastic](https://www.elastic.co/docs). Ela oferece guias completos, tutoriais e referências detalhadas sobre todos os recursos e funcionalidades disponíveis.

## 11. Funcionamento do Docker
-  **Execução de Containers**: No Migrador-Docker, há uma pasta cycle-controller que faz a execução da containerização da aplicação, usamos ssh para ativar-lo.
```bash
sh -T eXXXX-play.sh 
# Comando que usamos iniciar um arquivo shell
```
> Obs: Há um bug que pode acontecer algumas vezes que na execução desse arquivo na OP, é bom sempre verificar se estes arquivos abaixo estão configurado como Unix (LF).
Foi feito a mudança pelo notepad++, clicando com o botão direto e selecionando como Unix (LF), assim alterando o tipo de leitura do arquivo.

![unix](/assets/windowsCRLFtoUnixLF.png)

- Comandos básicos do Docker
```bash
## Iniciar um container
docker run -it ubuntu /bin/bash

## Listar containers em execução
docker ps

## Parar um container
docker stop <ID_CONTAINER>

## Remover um container
docker rm <ID_CONTAINER>

## Criar uma imagem
docker build -t minha-imagem .

## Listar imagens
docker images

## Remover uma imagem
docker rmi <ID_IMAGEM>
```

## 12. Casos do DIA-DIA.

1- Esta alteração do método **tratamento()** irá migrar os dados por API, quando a unidade territorial for UF, corretamente.

>Nota: Se atentar/corrigir os parâmetros enviados.


```java
private ArrayList<Map<String, Object>> tratamento(ArrayList<Map<String, Object>> listaDados, String urlDefinitiva,Map<String, Object> field, int totalRepete) {
        ArrayList<Map<String, Object>> listaDados2 = new ArrayList<>();
        Map<String, Map<String, Object>> ufMap = new HashMap<>();
        Map<String, Map<String, Object>> periodoMap = new HashMap<>();

        while (listaDados.size() > 0) {
            int total = 0;

            while (total < totalRepete && listaDados.size() > 0) {
                Map<String, Object> dado = listaDados.get(0);
                String uf = dado.get("D1N").toString();
                String periodo = dado.get("D3N").toString();

                String ufPeriodoKey = uf + "_" + periodo;

                Map<String, Object> docOut = ufMap.getOrDefault(ufPeriodoKey, new HashMap<>());
                docOut.put("uf", uf);
                docOut.put("periodo", periodo);

                ufMap.put(ufPeriodoKey, docOut);

                padronizaUf(docOut, uf);
                tratarNumero(dado, docOut,field);
                adicionarCamposPadrão(docOut, urlDefinitiva);

                listaDados.remove(0);
                total++;
            }
        }

        listaDados2.addAll(ufMap.values());
        return listaDados2;
    }
```
2- Use o fabricando caso queira iterar o fieldByType por nome.
```java
... 
  //Descomentar estes dois campos
  fieldNames = scheme.fabricandoFieldNames(row, separatorCharactere);
  fieldTypes = scheme.fabricandoFieldTypes(fieldNames);
...
  // Comentar estes dois campos
  fieldNames = scheme.fabricateFieldNames();
  fieldTypes = scheme.fabricateFieldTypes();
...
```
3- Padronizar o numero na variavel long.
>Se atentar/corrigir os parâmetros enviados
```java


//Descomentar no DataTransporter para conseguir mudar que são int/double convertando para long, nos que voce queira do fieldByType.
  ...
  camposLong = Arrays.asList(new String[]{"total", "quantidade", "campo2"});
  ...
```
## 13. Faça parte da nossa equipe, **contribua para o nosso crescimento**.

Este documento é uma diretriz para os processos de Engenharia de Dados da Consiste. Ele visa fornecer uma visão geral dos processos e procedimentos a serem seguidos pela equipe, garantindo a qualidade e a segurança dos dados coletados e processados.

Para contribuir com este documento, por favor, siga as seguintes etapas:

1. Leia o documento cuidadosamente e verifique se há alguma informação que precise ser atualizada ou corrigida.
2. Se você tiver alguma sugestão ou ideia para melhorar o documento, por favor, envie um e-mail para o coordenador da Engenharia de Dados.
3. Se você precisar fazer alguma alteração no documento, por favor, faça um fork do repositório e envie um pull request com as alterações.

Agradecemos sua contribuição!

[def]: #1-introdução
[def2]: #2-objetivos
[def3]: #3-programas-frameworks-e-bibliotecas-necessários
[def4]: #31-ferramentas-requeridas-na-máquina
[def5]: #311-visual-studio-code
[def6]: #312-python
[def7]: #313-java-e-jdk
[def8]: #314-eclipse
[def9]: #315-postman-e-elastic
[def10]: #316-git
[def11]: #317-notepad++
[def12]: #318-emditor
[def13]: #4-comandos-necessários-para-sobreviver
[def14]: #5-como-cortar-arquivos-rápido-sem-modificar
[def15]: #6-qual-migrador-usar
[def16]: #7-anotações-no-xtr-update
[def17]: #8-o-que-colocar-na-pasta-de-operações
[def18]: #9-rotina-de-versionamento-de-codigo
[def19]: #10-codigos-para-a-verifição-da-migração-dos-dados
[def20]: #11-funcionamento-do-docker
[def21]: #12-Casos-do-DIA-DIA
[def22]: #13-faça-parte-da-nossa-equipe-contribua-para-o-nosso-crescimento