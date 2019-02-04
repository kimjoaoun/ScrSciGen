# Script para raspar e classificar de Dados da Plataforma SciELO

Tendo como base dois pacotes desenvolvidos por @meirelesff, tive como ideia coletar os metadados disponibilizados pela plataforma SciELO e classificar eles por gênero. Para fazer a raspagem dos dados usei o package [rScielo](https://github.com/meirelesff/rScielo), para organiza-los foram utilizadas as ferramentas do Tidyverse e classificação dos nomes por gênero foi usado o package [genderBR](https://github.com/meirelesff/genderBR). O código possui algumas falhas, quais serão corrigidas, como por exemplo o fato dele responder NA para nomes estrangeiros (fácilmente explicado pelo fato da base de nomes utilizada pelo genderBR ser a do IBGE).

**Atenção: recomendo que execute o código com uma quantidade especifica de journals selecionados (será necessário alterá-lo para isso), já que a execução da raspagem de todos os dados disponíveis na SciELO pode demorar bastante.**

![Plot da Cont. Intl.](https://i.imgur.com/DPu6ri5.jpg)
