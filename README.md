[![PyPI - Solr](https://img.shields.io/badge/Solr-v8.9.0-orange)](https://solr.apache.org/)
[![PyPI - Java](https://img.shields.io/badge/OpenJDK-1.8-blueviolet)](https://openjdk.java.net/)
[![PyPI - Python](https://img.shields.io/badge/python-v3.6+-blue.svg)](https://pypi.org/project/bertopic/)
[![PyPI - License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/mediote/twAnalytics/blob/main/LICENSE)

# Apache Solr
O [Apache Solr](https://solr.apache.org/)(Searching On Lucene Replication) é um mecanismo de busca gratuito e de código aberto baseado na biblioteca Apache Lucene. Está disponível desde 2004 e é um dos mecanismos de pesquisa mais populares disponíveis hoje em todo o mundo. Solr, no entanto, é mais do que um mecanismo de busca - também é frequentemente usado como um banco de dados NoSQL baseado em documento com suporte transacional que pode ser usado para fins de armazenamento.
 
Escrito em Java, o Solr tem APIs RESTful XML / HTTP e JSON e bibliotecas de cliente para muitas linguagens de programação, como Java, Phyton, Ruby, C #, PHP e muitos mais, sendo usados para construir aplicativos de análise de big data e baseados em pesquisa para sites, bancos de dados, arquivos, etc.
 
O Solr recebe dados estruturados, semiestruturados e não estruturados de várias fontes, os armazena e indexa e os disponibiliza para pesquisa quase em tempo real. Solr também é usado por seus recursos analíticos, permitindo que você faça pesquisas facetadas de produtos, agregação de eventos de log / segurança, análises de mídia social e assim por diante.

 
### Quem usa

O Solr é usado como mecanismo de busca nas maiores empresas da Internet, provendo uma poderosa ferramenta de busca aos usuários. Entre essas empresas estão gigantes como a Apple, Netflix, Disney, AT&T, CNET, Cisco, AOL, NASA, MTV, Goldman Sachs, Cloudspace, Sears, GameSpot, eHarmony, TicketMaster, The Guardian, eBay, StubHub, IBM, Adobe, Best Buy, DuckDuckGo, Instagram e a Casa Branca (sede do governo dos EUA).

* Veja a [lista](https://wiki.apache.org/solr/PublicServers) de empresas que usam Solr.

### Recursos
Os principais recursos do Solr, incluem: busca textual, hit highlighting, busca facetada e analítica, indexação em tempo real, rich document parsing, busca geoespacial, extensive REST APIs bem como parallel SQL. Solr é de nível empresarial, seguro e altamente escalável, fornecendo pesquisa e indexação distribuída tolerante a falhas em escalas extremamente grandes de dados. 
Como o Solr é baseado em padrões abertos, ele é altamente extensível. As consultas Solr são solicitações HTTP simples e a resposta padrão é um documento no formato JSON, mas também pode ser em outros formatos, como: xml, csv, pdf, doc, docx, ppt, pptx, xls, xlsx, odt, odp, ods, ott, otp, ots, rtf, htm, html, txt e log. 
Isso significa que uma ampla variedade de clientes será capaz de usar o Solr, de outros aplicativos da web a clientes de navegador, aplicativos de cliente rico e dispositivos móveis. Qualquer plataforma capaz de HTTP pode se comunicar com o Solr. 
Instalação

 
# Instalação

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

Após configuradar o Solr como um serviço, podemos simplesmente usar os comandos abaixo para iniciar, parar e checar seu status: 

```bash
$ sudo service solr start
``` 
```bash
$ sudo service solr stop
``` 
```bash
$ sudo service solr status
``` 
