# VotaSP
App para ajudar a escolher candidatos a Deputado Estadual e Federal no estado de São Paulo.

## O que é o VotaSP?

O projeto VotaSP é a continuação do [Vota Campinas](http://votacampinas.org.br/), uma idéia que deu muito certo nas eleições para vereador de Campinas em 2016.

O principal objetivo do projeto é simplificar e facilitar o processo de escolha para os eleitores. Através de questões objetivas sobre saúde, educação, economia, segurança e outros temas, os eleitores podem verificar sua afinidade com os candidatos cadastrados. A afinidade é mostrada através de um ranking que compara as respostas priorizando as idéias mais parecidas.

O projeto é open source e, tudo o que está nele, é aberto para analise. Tentaremos também mostrar as regras envolvidas em todo o processo de maneira mais simples.

## Como funciona?

![Como funciona](como-funciona.png)

Após um breve cadastro, os usuários podem responder uma lista de 40 questões com o intuíto de entender suas posições políticas. São questões de temas diversos que abordam desde economia e políticas públicas até assuntos considerados mais polêmicos como liberação do porte de arma, legalização do aborto e descriminalização das drogas.

Os candidatos e os eleitores respondem as mesmas questões, tendo as seguintes opções de resposta:
 - Discordo plenamente
 - Discordo
 - Concordo
 - Concordo plenamente
 
Os canditados tem um campo adicional de justificativa em cada questão, podendo explicar (ou não) seus posicionamentos; A lista de respostas e as justificativas ficam públicas no perfil de cada um deles para consultas. 

### Como os candidatos respondem as questões?

Os candidatos devem se cadastrar com o e-mail e dados informados ao TSE, para evitar fraudes nas respostas. Todos passam por uma analise que compara o cadastro com a lista de candidatos liberada pelo TSE pré eleição. Após cadastro, é liberada uma lista de 40 questões em que todas devem ser respondidas (e podem ser justificadas). Caso o candidato não responda as 40 questões ele não estará apto a "dar match" com os eleitores e nem aparecerá nas buscas por seu nome dentro do app.

### Como os usuários respondem as questões?

O cadastro pode ser feito usando um e-mail ou as redes sociais. Após o cadastro é liberada uma lista de 40 questões em que o usuário deve responder no mínimo 20 para a realização do "match" com seu candidato. É importante ressaltar que quanto mais perguntas respondidas, mais assertivo será o resultado final.

Não é obrigatório responder todas as questões então, além das alternativas, há também um botão `pular`. É possivel voltar em questões puladas ou já respondidas para alterar a resposta.

## Como fazemos o match?

O Candidato pode responder com `Discordo plenamente`, `Discordo`, `Concordo`, `Concordo plenamente` enquanto o eleitor, além dessas alternativas, tem a opção de pular a questão (que desconsidera a questão no calculo final).

Para calcular o match:
  - Resposta igual = 2 pontos
  - Reposta distinta, porém concordante (discordo + discordo plenamente ou concordo + concordo plenamente) = 1 ponto
  - Respostas discordantes (concordo + discordo) = 0 pontos

Desenvolvemos uma [Prova de Conceito](https://github.com/Minhacps/votasp-poc-matcher) de como vai funciona o match internamente. Ajuda lá!

<br/>

## Como posso ajudar?

Nosso projeto é seguro e inclusivo, todos podem contribuir e são muito bem-vindos. Temos uma equipe mista e plural, acreditamos que todos podem contribuir para fazer o projeto crescer.

#### - Discord
Você pode ajudar simplesmente conversando e dando feedbacks no nosso [Discord](https://discord.gg/TGfXVHy).

#### - Desenvolvedores
O projeto já foi lançado mas sempre podemos melhorar para as próximas eleições. Já temos algumas estruturas de como o sistema deveria se comportar (olhe os repositórios de [front-end](https://github.com/Minhacps/votasp-app) e [back-end](https://github.com/Minhacps/votasp-backend) para entender melhor).

Você pode ajudar contribuindo com issues/pull-requests ou simplesmente aparecendo no nosso Discord pra conversar.

#### - Ajude a pressionar
Você também pode ajudar o projeto pressionando os candidatos que você conhece para que se cadastrem e preencham as questões. (Isso é muito importante para nós!)

#### - Ajude com custos do servidor
Você também pode nos ajudar com custos que nossos servidores tem. Estamos planejando uma arquitetura de microserviços e atualmente estamos rodando no Google Cloud.

Se você tem uma ferramenta que usamos, também pode ajudar facilitando os custos, como fizemos com o auth0, por exemplo.

<br/>

## Contribuição
Agradecemos por considerar contribuir com o VotaSP! Você encontra como fazê-lo em nosso [Guia de Contribuição](CONTRIBUTING.md).

<br/>

## Código de Conduta
Para garantir que a comunidade do VotaSP seja acolhedora para todos, leia e siga o nosso [Código de Conduta](CODE_OF_CONDUCT.md).

<br/>

## Licença
O VotaSP é um software de código aberto licenciado sob a [Licença MIT](LICENSE.md).
