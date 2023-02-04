# Muuvie
Repositório criado para acompanhamento da disciplina de Design de Software, ministrada pelo professor <i>Fabio Lucena</i>.

## Descrição
O objetivo deste projeto é o desenvolvimento de um sistema que coleta dados de plataformas de streaming, sites de avaliações de séries e filmes e de redes sociais, auxiliando na criação de perfis personalizados dos usuários das plataformas de streaming, a fim das mesmas direcionar seus serviços e propagandas de maneira mais eficaz.
<br>

## Muuvie - Seu filme em alguns muu's
Quem nunca se sentou na sala ou se deitou na cama e foi colocar um filme para assistir e se perguntou: _Qual o filme vou assistir hoje?_ E a partir desse momento você fica minutos, dependendo até horas passando por um catálogo até decidir o que assistir.

A ideia do nosso projeto é criar um serviço para ser utilizado por Plataforma de Streams. Neste serviço, através o recebimento de dados básicos demográficos de um determinado usuário e seu histórico de filmes assistidos, recomendaremos o filme ideal para que o usuário assista.

Foi inspirado em um protótipo realizado em outra disciplina para um aplicativo com mesmo nome porém com fluxo de utilização diferente.
Protótipo: [Link de acesso ao figma](https://www.figma.com/proto/3BouSZzPDmVwEkjrNSf8zA/app-muuvie?node-id=344%3A6533&starting-point-node-id=344%3A6533)
<br>

## Discentes
- Bruna Do Espirito Santo Sousa - Matrícula 202107999<br>
- Joyce Beatriz Ferreira Da Costa Silva - Matrícula 201910890<br>
- Layane Grazielle Souza Dias - Matrícula 202004763<br>
- Pedro Ivo Santana Melo - Matrícula 202004776<br>
- Pedro Paulo Oliveira Lopes - Matrícula 201905548

## Diagrama de contexto
Modelagem do escopo de forma gráfica, descrevendo as movimentações de dados e interações entre as interfaces do sistema.
![Diagrama de Contexto](Documentacao/DiagramaDeContexto.jpg)
## Diagrama de Contêiner
Agrupamento dos componentes do sistema em contêiners, detalhando de maneira macro o sistema de software, exibindo as várias partes do mesmo e mostrando as decisões de tecnologias decididas.
![Diagrama de Conteiner](Documentacao/DiagramaDeConteiner.jpg)
## Diagramas de Componentes

Componentes do Serviço para coleta e alocação de dados do Scraper de Redes Sociais.
![Diagrama de Componentes](Documentacao/DiagramaDeComponentesScraper.jpg)

Componentes do Serviço de refinamento dos dados coletados pelo Scraper de Redes Sociais. Esse dados serão utilizados para treinamento da Inteligência Artificial.

<b> Limpeza de Dados:</b> deve buscar por dados que contenham pelo menos 1 filme, informação de perfil demográfico e a qualificação sobre o(s) filme(s). Na ausência de alguma dessas informações será feito o descarte.

<b>Categoriza: </b> deve catalogar os dados para serem armazenados. 

![Diagrama de Componentes](Documentacao/DiagramaDeComponentesRefinamento.jpg)

Componentes do Serviço para coleta e alocação de dados da plataforma de avaliações e críticas de filmes.

![Diagrama de Componentes](Documentacao/DiagramaDeComponentesCriticos.jpg)
