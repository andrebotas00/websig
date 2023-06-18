# websig
Trabalho prático de websig

README - Guia de Início Rápido

Este documento fornece instruções para configurar e utilizar o sistema de mapeamento geoespacial descrito abaixo. Ele abrange a instalação de todas as dependências necessárias, configuração do servidor GeoServer, criação de estilos personalizados e publicação dos dados de mapas. Além disso, detalha a criação de um mapa interativo utilizando a biblioteca Leaflet.

Pré-requisitos

Antes de começar, certifique-se de ter os seguintes itens instalados em seu sistema:

PostGIS - Extensão geoespacial para o banco de dados PostgreSQL.

PostgreSQL - Sistema de gerenciamento de banco de dados relacional.

pgAdmin - Ferramenta gráfica para administração do PostgreSQL.

Apache Tomcat - Servidor web para executar o GeoServer.

GeoServer - Servidor de mapas para publicação e visualização de dados geoespaciais.

QGIS - Software de Sistemas de Informação Geográfica (SIG) para manipulação de dados geoespaciais.


Configuração do GeoServer

Siga as etapas abaixo para configurar o GeoServer:

Após instalar o Apache Tomcat, crie uma conta no Apache Tomcat seguindo as instruções do site.
Faça o download do GeoServer e instale-o no diretório apropriado do Apache Tomcat.
Inicie o Apache Tomcat e verifique se o GeoServer está sendo executado corretamente acessando http://localhost:8080/geoserver em seu navegador.
Conecte-se ao GeoServer usando as credenciais de administrador fornecidas durante a instalação.
Configuração do GeoServer e Publicação de Dados
Siga as etapas abaixo para carregar e publicar os dados geoespaciais no GeoServer:

No GeoServer, crie um "store" para cada camada de dados que deseja publicar. Importe os arquivos GeoJSON correspondentes localizados na pasta "Data".
Crie estilos personalizados para as camadas usando a funcionalidade de criação de "styles" no GeoServer.
Associe os estilos criados às camadas correspondentes em seus respectivos "stores".
Publique as camadas criadas no GeoServer.
Alternativamente, você também pode operar os dados no QGIS e, em seguida, carregar os dados manipulados para o servidor GeoServer seguindo as etapas acima.

Resumo do Projeto

O objetivo deste projeto foi criar um sistema de mapeamento geoespacial que exibisse informações sobre casos de COVID e estádios em Lisboa. O processo envolveu as seguintes etapas:

Configuração do ambiente: Foram instalados o PostGIS, PostgreSQL, pgAdmin e Apache Tomcat para suportar o GeoServer.

Configuração do GeoServer: O GeoServer foi instalado e configurado para funcionar corretamente no Apache Tomcat.

Carga de dados: Foram carregados dois conjuntos de dados no GeoServer - casos de COVID e localizações dos estádios em Lisboa. Esses dados estavam em formato GeoJSON e foram importados para "stores" no GeoServer.

Estilização dos mapas: Foram criados estilos personalizados no GeoServer para definir a aparência dos mapas. Esses estilos foram associados aos dados carregados anteriormente.

Publicação dos mapas: As camadas de dados foram publicadas no GeoServer, permitindo que fossem visualizadas e acessadas através de serviços web.

Criação do mapa interativo: Utilizando a biblioteca Leaflet, foi criado um arquivo HTML que exibia um mapa de Portugal com base no OpenStreetMap (OSM). Os dados de casos de COVID e estádios em Lisboa foram adicionados ao mapa. Também foi implementada uma funcionalidade de clustering para facilitar a análise espacial dos dados.

Organização do projeto: Os arquivos utilizados na criação do HTML, juntamente com o HTML e o próprio README, foram organizados em pastas específicas no projeto.

Estrutura do Projeto

O projeto é organizado da seguinte forma:

Data: Contém os arquivos de dados de casos de COVID e as localizações dos estádios no formato GeoJSON. Dados Covid fornecidos através de "https://covid19.min-saude.pt/".

DIST: Contém os arquivos resultantes da criação dos clusters, obtidos a partir do HTML.

IMG: Contém o ícone utilizado para representar os estádios no mapa.

js: Contém os resultados em JavaScript de algumas ações de mapeamento utilizando a biblioteca Leaflet.

Conclusão

Este guia fornece os passos iniciais para configurar e utilizar o sistema de mapeamento geoespacial descrito. Para obter mais informações e explorar recursos avançados, consulte a documentação oficial de cada uma das ferramentas mencionadas.

Aproveite a criação de mapas interativos e a análise espacial dos dados geoespaciais em seu projeto!
