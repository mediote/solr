# Introdução

Solr é uma plataforma de pesquisa de código aberto rápida desenvolvida sobre o Apache Lucene ™. Fornecendo pesquisa distribuída e replicação de índice, o Solr foi projetado para escalabilidade e tolerância a falhas. O Solr é amplamente usado para casos de uso de pesquisa e análise corporativa e tem uma comunidade de desenvolvimento ativa e versões regulares.
 
### Quem usa

O Solr é usado como mecanismo de busca nas maiores empresas da Internet, provendo uma poderosa ferramenta de busca aos usuários. Entre essas empresas estão gigantes como a Apple, Netflix, Disney, AT&T, CNET, Cisco, AOL, NASA, MTV, Goldman Sachs, Cloudspace, Sears, GameSpot, eHarmony, TicketMaster, The Guardian, eBay, StubHub, IBM, Adobe, Best Buy, DuckDuckGo, Instagram e a Casa Branca (sede do governo dos EUA).

* Veja a [lista](https://wiki.apache.org/solr/PublicServers) de sites que usam Solr.

### Recursos
Os principais recursos do Solr, incluem: busca textual, hit highlighting, busca facetada e analítica, indexação em tempo real, rich document parsing, busca geoespacial, extensive REST APIs bem como parallel SQL. Solr é de nível empresarial, seguro e altamente escalável, fornecendo pesquisa e indexação distribuída tolerante a falhas em escalas extremamente grandes de dados. 
Como o Solr é baseado em padrões abertos, ele é altamente extensível. As consultas Solr são solicitações HTTP simples e a resposta é um documento estruturado: principalmente JSON, mas também pode ser XML, CSV ou outros formatos, como: xml, json, csv, pdf, doc, docx, ppt, pptx, xls, xlsx, odt, odp, ods, ott, otp, ots, rtf, htm, html, txt e log. 
Isso significa que uma ampla variedade de clientes será capaz de usar o Solr, de outros aplicativos da web a clientes de navegador, aplicativos de cliente rico e dispositivos móveis. Qualquer plataforma capaz de HTTP pode se comunicar com o Solr. 
Instalação

 
# Instalação

O Solr pode ser instalado em sistemas GNU/Linux, macOS e Windows. Neste trabalho o Solr foi instalado no Ubuntu 20.04

### Passo 1 - Instalando o Java
O Solr é desenvolvido em Java, então será preciso instalar o Ambiente de Exucação Java (JRE ou Java Runtime Environment) 1.8 ou superior. 

```bash
$ jsudo apt install openjdk-11-jdk
``` 
Verificando se o Java já está instalado

```bash
$ java -version
``` 


### Passo 2 - Instalando o Solr no Ubuntu
O procedimento de instalação do Solr detalhado a seguir, foi executado no sistema operacional Ubuntu 20.04 e, basicamente, se resume a baixar e descompactar o Solr.
 
 Baixando o Solr
$ cd /opt
$ sudo wget https://downloads.apache.org/lucene/solr/8.9.0/solr-8.9.0.tgz
 
 Descompactando e instalando 

$ tar xzf solr-8.9.0.tgz solr-8.9.0/bin/install_solr_service.sh --strip-components=2
$ sudo bash ./install_solr_service.sh solr-8.9.0.tgz
Passo 3 - Start / Stop Solr 
$  sudo service solr stop
$  sudo service solr start
$  sudo service solr status
 
