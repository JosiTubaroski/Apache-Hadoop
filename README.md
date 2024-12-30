<div> 
<p><a href="https://github.com/JosiTubaroski/Introducao_Engenharia_Dados/blob/main/README.md">Introdução a Engenharia de Dados</a></p>
</div> 

# Apache Hadoop

## A História do Apache Hadoop

O Apache Hadoop tem uma história fascinante, que começa nos desafios do crescimento exponencial de dados na era digital. Seu surgimento está diretamente ligado a ideias revolucionárias publicados pelo Google e ao trabalho de engenheiros visionários.

### 1. A Inspiração: Os Artigos do Google

Nos anos 2000, o Google enfrentava problemas para processar e armazenar o volume crescente de dados gerados por seu mecanismo de busca. A solução veio na forma de dois artigos publicados por engenheiros do Google:

#### 1. Google File System (GFS):

  - Publicado em 2003.
  - Descrevia um sistema de arquivos distribuído, escalável e tolerante a falhas, projetado para armazenar grandes conjuntos de dados e operar em hardware comum.

#### 2. MapReduce:

  - Publicado em 2004.
  - Introduzia um modelo de programação para processamento paralelo de dados em larga escala.

Esses artigos se tornaram o ponto de partida para o desenvolvimento do Hadoop, pois detalhavam como resolver desafios relacionados ao armazenamento e processamento de Big Data.

### 2. Os Fundadores: Doug Cutting e Mike Cafarella

  - Doug Cutting e Mike Cafarella trabalhavam no projeto Nutch, um motor de busca de código aberto.
  - Eles perceberam que poderiam adaptar as ideias descritas nos artigos do Google para criar uma infraestrutura robusta para processamento de dados.
  - Em 2005, implementaram o MapReduce e um sistema de arquivos distribuído semelhante ao GFS dentro do Nutch.

### 3. O Nascimento do Hadoop

  - Em 2006, Doug Cutting separou a infraestrutura de processamento e armazenamento do Nutch, criando um projeto independente chamado Hadoop.
  - O nome "Hadoop" foi inspirado no elefante de pelúcia do filho de Doug Cutting, tornando-o icônico.

### 4. Adoção pelo Yahoo!

  - Em 2006, o Yahoo! contratou Doug Cutting para liderar o desenvolvimento do Hadoop.
  - A empresa precisava processar grandes volumes de dados gerados por suas operações online, e o Hadoop parecia ser a solução ideal.
  - Em 2008, o Yahoo! construiu um dos maiores clusters de Hadoop do mundo, com 10.000 nós, consolidando sua confiança na ferramenta.

### 5. Tornando-se um Projeto da Apache

  - Em 2008, o Hadoop foi aceito como um projeto de nível superior pela Apache Software Foundation.
  - Esse marco transformou o Hadoop em uma ferramenta de código aberto amplamente acessível, permitindo que empresas e desenvolvedores contribuíssem para seu crescimento.

### 6. Expansão do Ecossistema Hadoop

Com o tempo, o Hadoop deixou de ser apenas MapReduce e HDFS. Ele se tornou um ecossistema completo para processamento e gerenciamento de Big Data, com novos componentes e ferramentas, como:

 - YARN (Yet Another Resource Negotiator): Gerenciamento de recursos para clusters Hadoop.
 - Hive: Ferramenta para consultas SQL-like em dados armazenados no HDFS.
 - Pig: Linguagem de alto nível para análise de dados.
 - HBase: Banco de dados NoSQL.
 - Spark: Processamento em memória, integrado ao Hadoop.

## Impacto do Hadoop

O Hadoop revolucionou o mundo da tecnologia, oferecendo soluções para desafios como:

#### 1. Armazenamento Escalável:

 - O HDFS permite armazenar petabytes de dados em hardware comum.

#### 2. Processamento Paralelo:

 - O MapReduce acelera o processamento de grandes volumes de dados distribuindo as tarefas entre vários nós.

#### 3. Big Data Mainstream:

 - Empresas como Facebook, Twitter, LinkedIn, Netflix e Amazon adotaram o Hadoop para gerenciar seus dados.

#### 4. Base para Inovação:

 - Hadoop abriu caminho para o surgimento de ferramentas e frameworks como Apache Spark, Flink e Storm, que trouxeram novos paradigmas de processamento.

<img src="https://github.com/JosiTubaroski/Apache-Hadoop/blob/main/hadoop_Linha_Tempo.png">


### Resumo

O Hadoop nasceu da necessidade de lidar com Big Data de maneira escalável e eficiente, inspirado pelos desafios enfrentados pelo Google. Com apoio do Yahoo! e da comunidade de código, tornou-se a pedra angular para ambientes de engenharia de dados, transformando o armazenamento e processamento distribuído em um padrão da industria.


# Qual o primeiro projeto a utilizar o hadoop?

O primeiro projeto a utilizar o Hadoop foi o Nutch, um motor de busca de código aberto.

### Origem do Uso no Nutch

- Desafio no Nutch: O projeto Nutch, iniciado por Doug Cutting e Mike Cafarella em 2002, buscava construir uma alternativa de código aberto aos mecanismos de busca dominantes,
  como o Google.  Porém, à medida que o Nutch crescia, os desenvolvedores enfrentavam dificuldades para armazenar e processar grandes volumes de dados indexados de páginas da web.

- Inspiração dos Artigos do Google: Após a publicação dos artigos do Google File System (GFS) em 2003 e do MapReduce em 2004, Doug Cutting e Mike Cafarella perceberam que poderiam implementar soluções semelhantes para resolver os problemas do Nutch.

- Adaptação das Ideias: Em 2005, eles implementaram o MapReduce e um sistema de arquivos distribuído (que mais tarde se tornou o HDFS) dentro do Nutch.

### Separação do Hadoop do Nutch

- Em 2006, as partes de processamento distribuído (MapReduce) e armazenamento (HDFS) do Nutch foram extraídas e transformadas em um projeto independente chamado Hadoop.
- A separação permitiu que o Hadoop fosse usado como uma solução genérica para outros problemas de Big Data, além do mecanismo de busca.

## Importância do Nutch

O uso inicial no Nutch mostrou a viailidade do Hadoop para lidar com grandes volumes de dados de forma escalável e eficiente, abrindo caminho para sua adoção em outras áreas e sua popularização como um framework fundamental para Big Data.

# O que os mecanismos de busca tem em comum com a engenharia de dados?

Os mecanismos de busca e aengenharia de dados compartilham diversas características e objetivos, pois ambos lidam com o processamento, armazenamento e análise de grandes volumes de dados. Aqui estão os principais pontos em comum:

### 1 . Coleta de Dados

   - Mecanismos de Busca:

     - Rastreiam (crawl) páginas da web, coletando dados de conteúdo, estrutura e metadados para indexação.
     - Esse processo é semelhante a pipelines de extração de dados.
    
   -  Engenharia de Dados:

      - Envolve a extração de dados de fontes variadas, como APIs, bancos de dados, arquivos e streams.
    
### 2. Processamento de Dados 

   - Mecanismos de Busca:

     - Processam os dados para indexação e classificação, garantindo que as consultas sejam rápidas e precisas.
     - Utilizam algoritmos de ranqueamento, como o PageRank.
    
   - Engenharia de Dados:

     - Processa dados para transformá-los em formatos úteis, como tabelas normalizadas, agregações ou estruturas otimizadas para análise.

### 3. Armazenamento Escalável

  - Mecanismos de Busca:
    - Precisam armazenar vastas quantidades de informações sobre páginas da web, incluindo cópias do conteúdo, índices invertidos e metadados.
    - Engenharia de Dados:
      - Utiliza sistemas de armazenamento escaláveis (como Hadoop HDFS, S3, ou bancos de dados distribuídos) para lidar com grandes volumes de dados.

### 4. Uso de Modelos Distribuídos

   - Mecanismos de Busca:
     - Dividem tarefas como rastreamento, indexação e ranqueamento entre vários servidores, aproveitando a computação distribuída.

   - Engenharia de Dados:
     - Utiliza computação distribuída (Hadoop, Spark) para realizar processamento paralelo em grandes conjuntos de dados.
   
### 5. Consultas e Otimização

   - Mecanismos de Busca:
     - Respondem a consultas dos usuários rapidamente, com resultados precisos.
     - Utilizam índices invertidos para eficiência.
    
   - Engenharia de Dados:
     - Cria e otimiza estruturas de consulta em bancos de dados, data warehouses e lakes, garantindo que análises sejam rápidas e escaláveis.

### 6. Foco na Qualidade e Relevância dos Dados

   - Mecanismos de Busca:
     - Implementam estratégias para garantir que os resultados sejam relevantes e atualizados.
    
   - Engenharia de Dados:
     - Limpa, valida e normaliza dados para evitar inconsistências e melhorar a confiabilidade das análises.
    
### 7. Aplicação de Algoritmos e Machine Learning

  - Mecanismos de Busca:
    - Usam algoritmos de aprendizado de máquina para personalização, previsão de comportamento do usuário e melhoria de resultados.
   
  - Engenharia de Dados:
    - Prepara e entrega os dados necessários para treinar e testar modelos de machine learning.

### 8. Enfrentam os 3Vs do Big Data

   - Ambos enfrentam os desafios clássicos do Big Data:
     - Volume: Grandes quantidades de dados.
     - Velocidade: Necessidade de processar dados rapidamente.
     - Variedade: Diferentes formatos e tipos de dados.
    
## Conclusão

Mecanismos de busca, como Google e Bing, podem ser considerados grandes aplicações práticas de engenharia de dados. Eles usam conceitos de extração, transformação, armazenamento, indexação e análise de dados em larga escala, o que está diretamente alinhado com os princípios e ferramentas da engenharia de dados.
