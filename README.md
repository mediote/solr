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

## Terminologia do Solr: Compreendendo os conceitos básicos usados no Solr 

Antes de mergulhar no processo de funcionamento do Solr, é importante entender os termos-chave usados ao trabalhar com o Solr.

* <b>Documento:</b> Um documento é uma unidade básica de informação no Solr que pode ser armazenada e indexada. Os documentos são armazenados em coleções. Eles podem ser adicionados, excluídos e atualizados, normalmente por meio de manipuladores de índice.

* <b>Campo:</b> O campo armazena os dados em um documento que contém um par de chave-valores, onde a chave indica o nome do campo e o valor dos dados reais do campo. Solr suporta diferentes tipos de campo: float, long, double, date, date, text, integer, boolean, etc.

* <b>Coleção:</b> Uma coleção Solr é um grupo de fragmentos / núcleos que formam um único índice lógico. Cada coleção tem seu próprio conjunto de configuração e definição de esquema, que pode ser diferente de outras coleções.

* <b>Fragmento:</b> Os fragmentos permitem que você divida e armazene seu índice em uma ou mais partes, portanto, um fragmento é uma fatia de uma coleção. Cada fragmento vive em um nó e é hospedado em um núcleo.

* <b>Nó:</b> É uma única instância da JVM executando Solr, também conhecido como servidor Solr. Um nó pode hospedar vários fragmentos.

* <b>Réplica:</b> Uma réplica é uma cópia física de um shard executado como um núcleo em um nó. Uma dessas cópias é um líder (veja abaixo). Outras cópias do mesmo fragmento replicarão os dados do líder. Leia mais sobre os tipos de réplicas e replicação Solr aqui:

* <b>Líderes:</b> O líder é uma réplica do fragmento que envia solicitações do SolrCloud para o resto das réplicas no fragmento sempre que houver uma atualização de índice, como adições ou exclusões de documentos. Se o líder cair, uma das outras réplicas será eleita líder automaticamente.

* <b>Cacho:</b> Específico para SolrCloud, um cluster é composto de um ou mais nós que armazenam todos os dados, fornecendo indexação distribuída e recursos de pesquisa em todos os nós. Leia mais sobre SolrCloud aqui.

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

Se tudo ocorrer bem, a interface de administração do Solr pode ser acessada em http://localhost:8983.

## Como o Solr funciona?

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

As consultas no Solr, podem ser feitas diretamente pelo painel de administração, ou usando o manipulador de consulta. Através de uma requisição HTTP a URL
http://localhost:8983/solr/fsp/select?q.op=OR&q=TEXT%3A%20Ayrton%20Senna por exemplo, foi executada uma consulta sobre o campo "TEXT" usando como argumentos de busca os termos "Ayrton Senna". O retorno por padrão são os documentos com campos chave-valor no formato JSON conforme abaixo:

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
        "TEXT":["6 de maio de 94A Corusp (Associação dos Corredores de Rua de São Paulo) decide organizar uma maratona para homenagear o piloto Ayrton Senna, morto no dia 1º11 de agosto de 94Leonardo Senna e a direção da Corusp têm audiência com o prefeito Paulo Maluf, que dá apoio a maratona Ayrton Senna20 de outubro de 94O Diário Oficial do Município publica a portaria 174/94 oficializando a realização da Maratona Ayrton Senna no dia 25 de junho de 95Janeiro de 95Leonardo Senna se encontra com o diretor de esportes da Rede Globo, Cyro José, e apresenta a idéia da maratona Ayrton Senna. José diz que vai estudar a propostaMarço de 95Sem resposta da Globo, a Corusp e Leonardo Senna fecham acordo de transmissão com o SBT, que se propõe a viabilizar, através de anunciantes, a parte comercial da maratona18 de maio de 95Em reunião com a Corusp, o então secretário de Esportes, Arthur Alves Pinto, solicita a mudança de data da maratona para o dia 8 de outubro, para coincidir com a inauguração do túnel Ayrton Senna30 de maio de 95A Rede Globo solicita ao Inpi (Instituto Nacional de Propriedade Industrial) o registro para ela da marca \"Maratona Cidade de São Paulo\"13 de junho de 95Leonardo Senna e a Corusp têm nova audiência com o prefeito Maluf, que confirma a realização da prova e pede que eles se encontrem, no dia seguinte, com o secretário do Planejamento, Paulo Richter, para tratar dos detalhes14 de junho de 95Richter diz que a prefeitura já havia feito um acordo com a Globo para transmitir a maratona e informa que seu nome havia mudado para Maratona Cidade de São Paulo. Leonardo Senna e a Corusp não aceitam a mudança e se retiram da organização do evento5 de julho de 95A Confederação Brasileira de Atletismo envia uma carta aos organizadores da maratona autorizando a realização da prova no dia 8 de outubro13 de julho de 95A Rede Globo volta ao Inpi e solicita o registro de outra marca: \"Maratona de São Paulo\", que se tornaria o nome oficial da prova21 de julho de 95O prefeito Maluf assina decreto oficializando a Maratona de São Paulo, na mesma data em que estava agendada a Maratona Ayrton SennaAgosto de 95A prefeitura paga R$ 1,2 milhão à Rede Globo8 de outubro de 95Acontece a maratona Ayrton Senna. Ela é transmitida para todo o Brasil. Seu percurso passa pelas principais obras da prefeitura. O prefeito Paulo Maluf aparece várias vezes no ar. Nos intervalos, são veiculadas propagandas da prefeitura de São Paulo"],
        "id":"ee3e43ea-9821-4491-9142-3aebb5537485",
        "_version_":1711541907396493315},
      {
        "DOCID":["FSP950322-168"],
        "TEXT":["\"Pô! Deixei o sanduíche aí!\"De Ayrton Senna, por telefone, para Maurício Gugelmin, em 1982, quando os dois dividiam uma casa na Inglaterra. Senna havia esquecido em casa um sanduíche que tinha preparado especialmente para o dia de treinos.\"Fomos a uma boate, mas como eu era baixinho _nem 1,50 m eu tinha_ fiquei no carro esperando meu primo. Ele voltou com uma loiraça de 1,80 m. Até fiquei sem respiração e pensei: 'Tudo isso para mim?' Fomos para o apartamento dela. Não me assustei.\"De Ayrton Senna, sobre sua primeira aventura na noite paulistana, aos 13 anos.\"A maior parte do tempo, sou agressivo porque ainda não atingi o máximo aceitável e estou continuamente nessa perseguição. Talvez um dia, quando chegar a esse ponto, passe a ser menos agressivo e a ter um atitude mais calma e condescendente com a vida.\"De Ayrton Senna, sobre si mesmo.\"Uma volta rápida requer um alto nível de sensibilidade entre o corpo e a mente. É a combinação dos dois que dá a performance. Eu nunca consegui uma volta perfeita, porque eu sei, ao olhar para trás, que houve sempre lugar para melhoramentos. Não importa se é apenas um décimo ou um centésimo: há sempre espaço para melhorar.\"De Ayrton Senna, sobre pilotagem\"Dei o nome de Senna ao meu cachorro. Dou-lhe dois pontapés todo dia e sei que não irá chorar junto da imprensa.\"Nelson Piquet.\"Eu não aguento esse cara, parece que ele dorme no box: quando eu saio, ele fica lá; quando eu chego de manhã, ele já está lá...\"De Alain Prost, sobre Ayrton Senna\"Um p... carro daqueles e o cara fica chorando... Pinta o carro dele de vermelho e dá para mim...\"De Ayrton Senna, sobre Alain Prost, depois do GP da Inglaterra, em 1993.\"Infelizmente, a Xuxa gostava demais de sua profissão e não tínhamos tempo um para o outro. Tivemos que acabar, transformando-nos em grandes amigos.\"De Ayrton Senna, sobre o fim de seu namoro com Xuxa.\"Eles até dormiam no mesmo quarto...\"Do banqueiro Antônio Carlos de Almeida Braga, sobre o relacionamento de Senna com Marjorie Andrade, modelo brasileira que foi vista com o piloto em 1987.\"Eu tinha apenas uns 8 anos e a maioria dos outros tinha 16, 18, ou mesmo 20 anos. A forma de determinar as posições no grid era por sorteio. Punham uns papeizinhos com uns números dentro de um capacete. Por ser o mais novo, fui eu o primeiro a sortear. Tirei o número um.\"De Senna, sobre sua primeira corrida de Cart, uma corrida particular em que largou na pole-position.Declarações incluídas em \"Senna - The Face of a Champion\"."],
        "id":"5de2a1c9-19ab-48dd-932f-c77f8732ed42",
        "_version_":1711541900255690759},
      {
        "DOCID":["FSP950323-169"],
        "TEXT":["Livros, revistas, CD-ROM e até exposição informam aficionadosDa Reportagem Local Se você pretende ir ao GP do Brasil, existem diversas maneiras de ficar muito bem informado sobre a Fórmula 1 e entender tudo o que vai se passar no autódromo de Interlagos.Os anuários \"Fórmula 1\" e \"AutoMotor\" trazem todos os detalhes sobre a temporada de 95.O \"Fórmula 1\", de Francisco Santos, editado pela Edipromo, custa R$ 19.O \"AutoMotor\", da Casa Editorial, escrito por Flávio Gomes, sai por R$ 12.Entre as revistas especializadas, destacam-se a brasileira \"Grid\" (de periodicidade mensal), a inglesa \"Autosport\" e as italianas \"Autosprint\" e \"Auto e Sport\" (semanais).Todas elas trazem matérias sobre automobilismo esportivo em geral, com ênfase na Fórmula 1. A \"Grid\" custa R$ 3,50. Já o preço das estrangeiras varia de R$ 10 a R$ 20, de acordo com o estabelecimento onde sejam adquiridas.As livrarias Leonardo Da Vinci, La Selva e Siciliano dispõem, geralmente, das edições mais recentes das três publicações européias.Essas revistas chegam ao Brasil com uma semana de atraso em relação aos seus países de origem.Algumas bancas de jornais também costumam vender essas publicações, como a localizada na esquina da avenida Cidade Jardim com rua Groenlândia (Jardins, zona sul), a da praça Villaboim (Higienópolis, região central) e a do largo de Moema (zona sul).No rádio, os aficionados pela F-1 devem acompanhar o programa \"Pole Position\", aos sábados, às 13h, na Rádio Bandeirantes, com apresentação de Cândido Garcia.Existe também uma vasta bibliografia para quem quiser se aprofundar na história da categoria. A grande maioria dos livros disponíveis homenageia o piloto Ayrton Senna, morto no ano passado num acidente no autódromo de Imola, na Itália.O mais conhecido (e vendido) é \"Caminho das Borboletas\", um depoimento da modelo Adriane Galisteu, última namorada de Senna. O livro custa R$ 9.\"Ayrton Senna, Príncipe da Fórmula 1\", do jornalista australiano Ken Ryan, acaba de ser lançado no Brasil pela loja Speed Box Racing Club (rua Dr. Jesuíno Maciel, 1008, Campo Belo, zona sul de São Paulo). O preço promocional (temporário) é R$ 35. A compra pode ser feita por telefone (011-61-1457) ou pelo fax (011-542-6241).Também sobre Senna, escritos por jornalistas que acompanharam de perto a carreira do piloto, há: \"Recordando Ayrton Senna\", do inglês Alan Henry, e \"Ayrton Senna, Sua Vitória, Seu Legado\", da alemã Karin Sturm.Outros títulos: \"Ayrton Senna: a Face do Gênio\", do inglês Christopher Hilton, e \"Ayrton Senna do Brasil\", do português Francisco Santos.Já \"Fórmula 1, pela Glória e pela Pátria\", de Eduardo Correa, conta histórias de bastidores da categoria desde que os brasileiros começaram a se destacar, no início dos anos 70, com Emerson Fittipaldi.Os fãs de Ayrton Senna também podem saber mais sobre seu ídolo com a biografia do piloto em CD-ROM, lançado pelo empresa MicroPower. Em 70 minutos de programa, o usuário tem acesso, entre outras coisas, a depoimentos do piloto e ao \"Tema da Vitória\", marca registrada das corridas vencidas por Senna.O software está disponível através da CI-Distribuição (tel. 011-257-0577), ao preço de R$ 79.E, para entrar de vez no clima da Fórmula 1, você pode ir à exposição \"Reflexões de uma Trajetória Homenagem a Ayrton Senna\", do artista plástico Paulo Solaris.A mostra reúne 20 telas inéditas sobre a carreira do piloto e é dividida em cinco partes: \"O Sonho\", \"A Promessa\", \"A Batalha\", \"O Momento\" e \"A Consagração\".Essa exposição pode ser visitada até o próximo sábado, no Terraço Transamérica do Hotel Transamérica (av. das Nações Unidas, 18.591, Morumbi, zona sul)."],
        "id":"4be9a905-103a-4f0d-b350-9a7dd04a5e91",
        "_version_":1711541900276662278},
```

### Passo 3 - Ranqueamento

O Solr classifica os resultados por sua pontuação de relevância - os resultados mais relevantes aparecem no topo dos documentos correspondidos.
