# Princípio da responsabilidade única


O <b>Serviço de Scraper</b> é responsável por receber os dados das redes sociais. Cada componente desse serviço possui uma única responsabilidade, um recebe o dado, outro armazena no banco de dados e outro faz o descarte do banco de dados depois de 24 horas armazenado.
O <b>Serviço de Refinamento de Dados</b> é responsável por buscar dados relevantes para treinamento da Inteligência Artificial. Cada componente desse serviço possui uma única responsabilidade: a limpeza dos dados, que busca por dados que contenham pelo menos 1 filme, informação de perfil demográfico e a qualificação sobre o(s) filme(s), na ausência de alguma dessas informações será feito o descarte; e outro componente categoriza para armazenar em outro banco de dados.
O <b>Serviço de Coleta da Plataforma de Críticas e Avaliações de filmes</b> é responsável por receber os dados. Cada componente possui uma única responsabilidade: um para receber e outro para armazenar no banco de dados que será usado para a recomendação na plataforma de streaming.
