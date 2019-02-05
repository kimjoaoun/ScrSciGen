# Script para raspar e classificar de Dados da Plataforma SciELO

Tendo como base dois pacotes desenvolvidos por @meirelesff, tive como ideia coletar os metadados disponibilizados pela plataforma SciELO e classificar eles por gênero. Para fazer a raspagem dos dados usei o package [rScielo](https://github.com/meirelesff/rScielo), para organiza-los foram utilizadas as ferramentas do Tidyverse e classificação dos nomes por gênero foi usado o package [genderBR](https://github.com/meirelesff/genderBR).
O código possui algumas falhas, quais serão corrigidas:
* O fato dele responder NA para nomes estrangeiros (fácilmente explicado pelo fato da base de nomes utilizada pelo genderBR ser a do IBGE).
* Ele só identifica publicações feitas por um autor, publicações com mais de um autor são filtradas.

**Atenção: recomendo que execute o código com uma quantidade especifica de journals selecionados (será necessário alterá-lo para isso), já que a execução da raspagem de todos os dados disponíveis na SciELO pode demorar bastante.**

Por meio do código é possível gerar visualizações que mostram a quantidade de publicações feitas por homens e mulheres em determinadas publicações, na imagem abaixo é possível ver quando executado na revista Contexto Internacional (em 04/02). O código pode ser alterado para que se adicione nas visualizações mais detalhes, como o ano de publicação dos artigos.
![Plot da Cont. Intl.](https://i.imgur.com/DPu6ri5.jpg)
![Plot da Cont. Intl. 2](https://i.imgur.com/WMczwkV.jpg)
![Plot da Cont. Intl. 3](https://i.imgur.com/uzIfDBF.jpg?1)
