# Apache Solr

O Apache Solr é uma plataforma de pesquisa de código aberto rápida desenvolvida sobre o Apache Lucene ™. Fornecendo pesquisa distribuída e replicação de índice, o Solr foi projetado para escalabilidade e tolerância a falhas. O Solr é amplamente usado para casos de uso de pesquisa e análise corporativa e tem uma comunidade de desenvolvimento ativa e versões regulares.
 
### Quem usa

O Solr é usado como mecanismo de busca nas maiores empresas da Internet, provendo uma poderosa ferramenta de busca aos usuários. Entre essas empresas estão gigantes como a Apple, Netflix, Disney, AT&T, CNET, Cisco, AOL, NASA, MTV, Goldman Sachs, Cloudspace, Sears, GameSpot, eHarmony, TicketMaster, The Guardian, eBay, StubHub, IBM, Adobe, Best Buy, DuckDuckGo, Instagram e a Casa Branca (sede do governo dos EUA).

* Veja a [lista](https://wiki.apache.org/solr/PublicServers) de sites que usam Solr.

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
