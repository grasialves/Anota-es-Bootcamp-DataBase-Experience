# Anotações-Bootcamp-DataBase-Experience


**Introdução ao Banco de Dados**

* **O que são bancos de dados?**
    * Coleções de dados inter-relacionados
    * Exemplos: salas de arquivos, agendas de consultórios, MySQL, MongoDB, etc.
* **Siglas:**
    * SGBD (Sistema de Gerenciamento de Banco de Dados)
    * DBMS (Data Base Management System)
    * LDD (Linguagem de Definição de Dados)
    * HPC (High Performance Computing)
    * NoSQL (Not Only SQL)
* **Modelos de BDs:**
    * Relacional (Edgar F. Codd, 1970) - Baseado na álgebra relacional
    * Hierárquico - Estrutura de dados em árvore
    * Rede - Estrutura em links
* **Escolhendo SGBDs SQL ou NoSQL:**
    * Popularidade, tempo de mercado, documentação, robustez, confiabilidade, segurança, multiplataforma
* **Paradigmas:**
    * Empírico (tentativa e erro)
    * Teórico (teorema e axioma)
    * Computacional (simulações computacionais)
    * Big Data (análise e exploração de dados)
* **Diferença entre Big Data e HPC:**
    * Processamento paralelo persistente e não persistente e modelos associados

**Explorando a Abordagem de SGBDs**

* **Siglas:**
    * OLTP (Online Transaction Processing)
    * OLAP (Online Analytical Processing)
    * ELT (Extract, Load e Transform)
* **Abordagem de DBs:**
    * **BDs** Manter em DB
        * Abstração, auto-descrição, isolamento, compartilhamento, múltiplas visões, transação multiusuário
    * **Tradicional** Manter em arquivos
        * Complicações em redundância e esforço repetitivo
* **Auto-descrição:**
    * DBs: Descrição da estrutura e constraints
    * NoSQL: Descrição dentro do arquivo
* **Isolamento de dados e programa:**
    * DBs: Modificação no catálogo sem impactar a aplicação
    * Tradicional: Modificação acarreta em reestruturação
* **Múltiplas Visões:**
    * Table Views: Visualização segmentada ou sumarizada
* **Compartilhamento e Processamento de transações:**
    * Controle de Concorrência
    * OLTP: Transações, app multiusuário, gerador: Transações concorrentes, execução sem interferência, isolamento, atomicidade
    * OLAP: Análises de dados
    * ELT Process: Data mining, análise, decisão
* **Atores no cenário de DBs:**
    * DBs Simples
    * Big Organizations
    * Perfis:
        * **DB Designer** Modelagem
        * **DBA Staff** Administrador
        * **Usuários Finais** Users
* **Workers - background:**
    * Designer do sistema de SGBD
    * Implementação do sistema de SGBD
    * Pessoal de Operações e Manutenção
    * Desenvolvedores de ferramentas
* **Vantagens da abordagem de SGBDs:**
    * Controle de Redundância
    * Restrição de acesso
    * Storage - prove persistência
    * Storage - prove estrutura
    * Backup e Recovery
    * Prover interface Multi-user
    * Integridade de dados
    * Ganhos com SGBD
        * Padronização
        * Redução de tempo no desenvolvimento da aplicação
        * Flexibilidade
        * Disponibilidade de informação atualizadas
        * Economia com escalabilidade
* **Quando não utilizar SGBDs:**
    * Custo-benefício
    * Custo de overhead
    * Situações

**Overview sobre Modelagem de Dados**

* **O que é modelagem:**
    * Descrição e relacionamento dos elementos que compõem a representação do contexto (mini-mundo)
    * Processos da Modelagem:
        * Mini-mundo
        * Alto nível
        * Esquema
        * SGBD
* **Como inserir as informações no BD:**
    * SQL Linguagem declarativa
* **Como acessar:**
    * Clientes GUI
    * Clientes terminal

**Arquitetura de Banco de Dados**

* **Siglas:**
    * DDL (Data Definition Language)
    * SDL (Linguagem de Definição de Armazenamento)
    * VDL (Linguagem de Definição de Visões)
    * DCL (Linguagem de Controle de Dados)



## Anotações sobre NoSQL

**Modelos de Dados NoSQL:**

* **Chave-Valor (Key-Value):**
    * Armazena dados como pares de chave-valor.
    * Ideal para dados não estruturados ou semiestruturados.
    * Exemplos: DynamoDB, Redis, Riak.
* **Documentos:**
    * Armazena dados como documentos JSON, BSON ou XML.
    * Flexíveis e escaláveis.
    * Ideal para armazenar e recuperar documentos completos.
    * Exemplos: MongoDB, CouchDB, RavenDB.
* **Grafo:**
    * Armazena dados como grafos, com nós e arestas.
    * Ideal para relacionamentos complexos e análises de redes.
    * Exemplos: Neo4j, OrientDB, FlockDB.
* **Coluna:**
    * Armazena dados em colunas, similar a um spreadsheet.
    * Ideal para grandes volumes de dados com colunas pré-definidas.
    * Exemplos: Cassandra, HBase, ScyllaDB.

**Características dos Bancos de Dados NoSQL:**

* **Esquema Flexível:**
    * Adaptam-se a mudanças nos dados sem necessidade de modificações no banco de dados.
* **Escalabilidade Horizontal:**
    * Distribuem dados em vários servidores, aumentando a capacidade de processamento e armazenamento.
* **Alta Disponibilidade:**
    * Replicação de dados para garantir acesso mesmo em caso de falhas.
* **Consistência Eventual:**
    * As atualizações em diferentes servidores podem não ser instantâneas, mas eventualmente se sincronizam.
* **Sem ACID:**
    * Alguns modelos NoSQL não oferecem transações ACID (Atomicidade, Consistência, Isolamento e Durabilidade) completas.

**Aplicações Comuns de Bancos de Dados NoSQL:**

* **Redes Sociais:**
    * Armazenamento de perfis de usuários, conexões e publicações.
* **Comércio Eletrônico:**
    * Catálogos de produtos, carrinhos de compras e históricos de pedidos.
* **Internet das Coisas (IoT):**
    * Armazenamento e análise de dados de sensores e dispositivos.
* **Mídias Sociais:**
    * Armazenamento de fotos, vídeos e mensagens.
* **Aplicações Móveis:**
    * Sincronização de dados offline e geolocalização.

**Vantagens dos Bancos de Dados NoSQL:**

* **Flexibilidade:**
    * Ideal para dados não estruturados ou semiestruturados.
* **Escalabilidade:**
    * Suportam grandes volumes de dados e usuários.
* **Alto Desempenho:**
    * Processamento rápido de consultas e operações de leitura e gravação.
* **Disponibilidade:**
    * Redução do tempo de inatividade e tolerância a falhas.
* **Custo-Eficiência:**
    * Soluções de código aberto e opções de hospedagem na nuvem.

**Desvantagens dos Bancos de Dados NoSQL:**

* **Consistência Eventual:**
    * As atualizações em diferentes servidores podem não ser instantâneas.
* **Falta de ACID:**
    * Alguns modelos NoSQL não oferecem transações ACID completas.
* **Complexidade:**
    * Curva de aprendizado mais alta para alguns modelos.
* **Menos Padronização:**
    * Diversidade de modelos e ferramentas pode dificultar a escolha.

**Escolhendo entre SQL e NoSQL:**

* **SQL:**
    * Ideal para dados estruturados, transações ACID e consultas complexas.
    * Exemplos: Sistemas bancários, ERP, contabilidade.
* **NoSQL:**
    * Ideal para dados não estruturados, escalabilidade e flexibilidade.
    * Exemplos: Redes sociais, IoT, Big Data.

**Lembre-se:**

* A escolha entre SQL e NoSQL depende das necessidades específicas da sua aplicação.
* Avalie os prós e contras de cada modelo antes de tomar uma decisão.
* Existem ferramentas e serviços disponíveis para auxiliar na migração de dados entre SQL e NoSQL.

    
