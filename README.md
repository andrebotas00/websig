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

Criação do Mapa Interativo
Siga as etapas abaixo para criar um mapa interativo utilizando a biblioteca Leaflet:

Crie um arquivo HTML e utilize a biblioteca Leaflet, juntamente com CSS e JavaScript, para escrever o código do mapa.
No mapa, adicione uma camada de base do OpenStreetMap (OSM) para exibir o mapa de Portugal.
Adicione dados de casos de COVID e casos de COVID por 10 mil habitantes no mapa. Esses dados podem ser obtidos a partir dos arquivos GeoJSON localizados na pasta "Data".
Adicione ícones para representar os 3 estádios em Lisboa. O ícone correspondente pode ser encontrado na pasta "IMG".
Crie uma base de clusters para facilitar a análise espacial dos dados.
Salve o arquivo HTML criado.

Estrutura do Projeto
O projeto é organizado da seguinte forma:

Data: Contém os arquivos de dados de casos de COVID e as localizações dos estádios no formato GeoJSON.
DIST: Contém os arquivos resultantes da criação dos clusters, obtidos a partir do HTML.
IMG: Contém o ícone utilizado para representar os estádios no mapa.
js: Contém os resultados em JavaScript de algumas ações de mapeamento utilizando a biblioteca Leaflet.

Conclusão
Este guia fornece os passos iniciais para configurar e utilizar o sistema de mapeamento geoespacial descrito. Para obter mais informações e explorar recursos avançados, consulte a documentação oficial de cada uma das ferramentas mencionadas.

Aproveite a criação de mapas interativos e a análise espacial dos dados geoespaciais em seu projeto!
