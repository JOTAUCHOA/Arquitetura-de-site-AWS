# Arquitetura-de-site-AWS
Uma arquitetetura utilizand componentes da AWS para funcionar.

Essa arquitetura utiliza 6 componentes:
1º e 2º são representados pelo usuário(computador) e requisição(imagem de arquivo), no qual ele
faz uma requisição ao item chamado "Internte Getway" da AWS para conseguir acessar a aplicação.
Logo após que requisição é permitida, ela acessa a VPC no item "Getway VPC", para entrar na rede correta
da aplicação, pois a rede, além do fato que essa rede está configurada na região us-west-2 da AWS.
Quando dentro da rede, o item "S3" recebe as informações, que passa para a maquina "EC2" para processamento 
que consulta no banco "RDS" o website, que quando achado, retorna a tela do usuário a resposta de acesso a aplicação.
