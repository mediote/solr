[![PyPI - Solr](https://img.shields.io/badge/Solr-v8.9.0-orange)](https://solr.apache.org/)
[![PyPI - Java](https://img.shields.io/badge/OpenJDK-1.8-blueviolet)](https://openjdk.java.net/)
[![PyPI - Python](https://img.shields.io/badge/python-v3.6+-blue.svg)](https://pypi.org/project/bertopic/)
[![PyPI - License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/mediote/twAnalytics/blob/main/LICENSE)

# Apache Solr
O [Apache Solr](https://solr.apache.org/)(Searching On Lucene Replication), é um mecanismo de busca gratuito de código aberto, baseado na biblioteca Apache Lucene. Está disponível desde 2004, e é um dos mecanismos de pesquisa mais populares disponíveis hoje em todo o mundo. O Solr, no entanto, é mais do que um mecanismo de busca, também é frequentemente usado como um banco de dados NoSQL baseado em documento, com suporte transacional que pode ser usado para fins de armazenamento.
 
Escrito em Java, o Solr tem APIs RESTful XML / HTTP e JSON e bibliotecas de cliente para muitas linguagens de programação, como Java, Phyton, Ruby, C #, PHP e muitos mais, sendo usados para construir aplicativos de análise de big data e baseados em pesquisa para sites, bancos de dados, arquivos, etc.
 
O Solr recebe dados estruturados, semiestruturados e não estruturados de várias fontes, os armazena e indexa e os disponibiliza para pesquisa quase em tempo real. Solr também é usado por seus recursos analíticos, permitindo que você faça pesquisas facetadas de produtos, agregação de eventos de log / segurança, análises de mídia social e assim por diante. Tem suporte para arquitetura multi-tenant que permite dimensionar, distribuir e gerenciar índices para aplicativos de grande escala.

As consultas no Solr, são solicitações HTTP simples e a resposta padrão é um documento no formato JSON, mas também pode ser XML, CSV ou outros formatos, como: xml, csv, pdf, doc, docx, ppt, pptx, xls, xlsx, odt, odp, ods, ott, otp, ots, rtf, htm, html, txt e log. Isso significa que uma ampla variedade de clientes será capaz de usar o Solr, de outros aplicativos da web a clientes de navegador, aplicativos de cliente rico e dispositivos móveis. Qualquer plataforma capaz de HTTP pode se comunicar com o Solr. 

Resumindo, o Solr é uma plataforma de pesquisa estável, confiável e tolerante a falhas com um rico conjunto de funções básicas que permitem melhorar a experiência do usuário e a modelagem de dados subjacente. Por exemplo, entre as funcionalidades que ajudam a oferecer uma boa experiência do usuário, podemos nomear verificação ortográfica, pesquisa geoespacial, facetação ou sugestão automática, enquanto os desenvolvedores de back-end podem se beneficiar de recursos como junções, agrupamento, capacidade de importar formatos de documentos ricos e muitos mais.

No entanto, para entender completamente como usá-lo, abaixo estão alguns dos principais recursos do Solr:

## Recursos

* <b>Full-text Search:</b> O Solr fornece recursos avançados de pesquisa em tempo real,como pesquisa por campo, consultas booleanas, consultas de frase, consultas difusas, verificação ortográfica, curingas, junções, agrupamento, preenchimento automático e muito mais em diferentes tipos de dados.

* <b>Interfaces de administração:</b> Interface web responsiva integrada que permite que você execute tarefas administrativas, como gerenciamento de registro, adição, exclusão, atualização ou pesquisa de documentos.

* <b>Alta escalabilidade e flexibilidade:</b> Ferramentas como o Apache ZooKeeper, permitem escalar o Solr, com replicação de índice automatizada, distribuição, balanceamento de carga e failover e recuperação automatizados. Portanto, dependendo das necessidades e do tamanho de sua operação, o Solr pode ser implantado em qualquer tipo de sistema, como autônomo, distribuído, nuvem, tudo isso ao mesmo tempo em que simplifica a configuração.

* <b>Suporte multilíngue:</b> Além do inglês, o Solr trabalha com vários outros idiomas, como chinês, japonês, coreano, árabe, alemão, francês, espanhol e muitos outros. Possui detecção de idioma embutida e fornece ferramentas de análise de texto específicas para cada idioma.

## Termos-chave 

É importante entender alguns termos-chave usados para iniciar o aprendizado do Solr.

* <b>Document :</b>A unidade básica de informação do Solr é um documento, que é um conjunto de dados que descreve algo. 

* <b>Field :</b>No universo Solr, os documentos são compostos por campos, que são informações mais específicas.

* <b>Core :</b>No Solr, o termo núcleo é usado para se referir a um único índice.


## Principais aquivos

### solrconfig.xml

É o arquivo de configuração com a maioria dos parâmetros que afetam o próprio Solr.

Através dele você configura recursos importantes, como:

* request handlers, que processam as solicitações ao Solr, como solicitações para adicionar documentos ao índice ou solicitações para retornar resultados para uma consulta
* listeners, processos que "ouvem" eventos específicos relacionados à consulta; podem ser usados para criar gatilhos e executar algum código, como invocar algumas consultas comuns para criar caches
* request dispatcher para gerenciar comunicações HTTP
* interface da Web de administração
* parâmetros relacionados à replicação e duplicação (esses parâmetros são abordados em detalhes em Legacy Scaling and Distribution)

### managed-schema ou schema.xml
Este aquivo informa ao Solr o que fazer com os dados recebidos ao construir um índice ou realizar uma query. Define como o Solr deve interpretar os dados em um campo e como o campo pode ser consultado; como analisar tokenizar ou filtrar os dados ou ainda aplicar stemmers, remoção de stop-words dentre outros.


## Quem usa

O Solr é usado como mecanismo de busca nas maiores empresas da Internet, provendo uma poderosa ferramenta de busca aos usuários. Entre essas empresas estão gigantes como a Apple, Netflix, Disney, AT&T, CNET, Cisco, AOL, NASA, MTV, Goldman Sachs, Cloudspace, Sears, GameSpot, eHarmony, TicketMaster, The Guardian, eBay, StubHub, IBM, Adobe, Best Buy, DuckDuckGo, Instagram e a Casa Branca (sede do governo dos EUA).

* Veja a [lista](https://wiki.apache.org/solr/PublicServers) de empresas que usam Solr.

## Instalação

O Solr pode ser instalado em sistemas GNU/Linux, macOS e Windows. Neste trabalho, foi instalada a versão 8.9.0 do Solr foi no sistema operacional Ubuntu 20.04

### Passo 1 - Instalando o Java

Você precisará do Java Runtime Environment (JRE) versão 1.8 ou superior. Em uma linha de comando, verifique sua versão do Java desta forma:

```bash
$ java -version
``` 
A saída exata irá variar, mas você precisa se certificar de que atende ao requisito mínimo de versão. O Java está disponível em vários provedores. São recomendadas as versões OpenJDK e Oracle do Java. Alguns são gratuitos, outros têm um custo, alguns fornecem patches de segurança e suporte, outros não. Para instalar a JRE, execute o comando a seguir:

```bash
$ sudo apt install openjdk-11-jdk
``` 

Com a JRE instalada corretamente, podemos prosseguir para os prórximos passos da instalação.

### Passo 2 - Instalando o Solr no Ubuntu
O procedimento de instalação do Solr detalhado a seguir, foi executado no sistema operacional Ubuntu 20.04, e basicamente, se resume a baixar e descompactar o Solr em algum diretŕorio de sua preferência.

```bash
$ cd /opt
``` 
```bash
$ sudo wget https://downloads.apache.org/lucene/solr/8.9.0/solr-8.9.0.tgz
``` 

Após baixado, os comandos a seguir, extraem e instalam o solr como um serviço no sistema operacional.

```bash
$ tar xzf solr-8.9.0.tgz solr-8.9.0/bin/install_solr_service.sh --strip-components=2
``` 
```bash
$ sudo bash ./install_solr_service.sh solr-8.9.0.tgz
``` 

### Passo 3 - Solr Start / Stop / Status 

Após configurar o Solr como serviço, podemos simplesmente usar os comandos abaixo para iniciar, parar e checar seu status: 

```bash
$ sudo service solr start
``` 
```bash
$ sudo service solr stop
``` 
```bash
$ sudo service solr status
``` 

Se tudo ocorrer bem, a interface de administração do Solr pode ser acessada em http://localhost:8983.

## Solr na prática

Solr funciona reunindo, armazenando e indexando documentos de diferentes fontes e tornando-os pesquisáveis quase em tempo real. Ele segue um processo de 3 etapas que envolve indexação, consulta e, finalmente, ranqueamento dos resultados - tudo em tempo quase real, embora possa funcionar com grandes volumes de dados.

Mais especificamente, aqui está como Solr executa as seguintes operações em uma sequência para pesquisar um documento:


### Passo 1 - Indexação de Arquivos

Execute o comando abaixo para criar a coleção usando levando em consideração o diretório no qual o Solr foi instalado:

```bash
$ sudo su - solr -c "/opt/solr/bin/solr create -c minhacolecao -n data_driven_schema_configs"
``` 

O Solr inclui a ferramenta em bin/post para facilitar a indexação de vários tipos de documentos. Execute comando abaixo para indexar os arquivos:

```bash
$ /opt/solr/bin/post -c meusarquivos diretoriodosarquivos/*
``` 

### Passo 2 - Consulta 

As consultas no Solr, podem ser feitas diretamente pelo painel de administração, ou usando o manipulador de consulta. Através de uma requisição HTTP a URL http://localhost:8983/solr/fsp/select?q.op=OR&q=TEXT%3AAyrton%20Senna por exemplo, foi feita uma consulta sobre o campo "TEXT" usando como argumentos de busca os termos "Ayrton Senna". O retorno por padrão são os documentos mais relevantes com campos chave-valor no formato JSON conforme abaixo:

```json
{
  "responseHeader":{
    "status":0,
    "QTime":0,
    "params":{
      "q":"TEXT: Ayrton Senna",
      "q.op":"OR",
      "_":"1632428094264"}},
  "response":{"numFound":288,"start":0,"numFoundExact":true,"docs":[
      {
        "DOCID":["FSP951020-097"],
        "TEXT":["6 de maio de 94A Corusp ......."],
        "id":"ee3e43ea-9821-4491-9142-3aebb5537485",
        "_version_":1711541907396493315},
      {
        "DOCID":["FSP950322-168"],
        "TEXT":["\"Pô! Deixei o sanduíche aí!\"De Ayrton Senna, ....."],
        "id":"5de2a1c9-19ab-48dd-932f-c77f8732ed42",
        "_version_":1711541900255690759},
```

### Passo 3 - Ranqueamento

O Solr classifica os resultados por sua pontuação de relevância - os resultados mais relevantes aparecem no topo dos documentos correspondidos.
