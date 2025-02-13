# Aula 3

Então nessa aula agora a gente vai verificar. A gente vai usar o explorador da Optimism, a Optimism explorer. Explore mais especificamente a testnet Optimism explorer e a gente vai começar a visualizar as transações que a gente está realizando dentro do nosso código aqui. Quem está desenvolvendo, tá? Então vão aqui pra tela. Eu atualizei o endereço daquele goerli.optimism.io, tá?

A private key que a gente vai vai colocar dessa forma, porque a gente vai trabalhar com Arquivo Environment, tá? E dentro desse arquivo enviroment não tem problema mostrar essa chave privada, porque eu não uso ela para nada. Tá, acabei de gerar. Mas lembre se que para chave precisa você sempre precisa manter segurança, tá? Então essa prova de que que você vai colocar tua parte que é para ver de quem que está subindo contrato inteligente, tá?

E aí a gente trabalha dessa forma, tá? Lembre se de instalar  dotenv, tá? Se eu vier aqui no terminal instalar o dote assim, dessa forma date ele que é pra gente utilizar hoje as dependências, que é para a gente utilizar o arquivo para utilizar variáveis dentro do .env. Bom, dito isso, é um bom tentar fazer alguns testes aqui, mas se eu vir aqui e colocar”yarn hardhat run scripts/deploy” supostamente deveria fazer o deploy —  utilizando aquela private key — do contrato.

Está isso aqui, o endereço do contrato. Vamos lá, dá uma olhada no Explorer, tá? Se vocês não tiverem com Meta Mask, é só clicar aqui nesse botãozinho para colocar o e colocar essa blockchain, essa testnet no teu Metamask. Mas eu vou colocar o endereço daquele contrato que foi emulado, tá? Então eu copiei esse endereço 0x5F e vou colar aqui, pra ver o que eu consigo localizar.

Engraçado que ele parece que já é como se já tivesse se esse contrato já tivesse sido feito. Vamos jogar mais uma vez aqui, que foi lá que ele vai ter que jogar um novo o novo contrato, certo? Ele vai ter que colocar um novo endereço de contrato. Ah, ele tá sim, sim, ele tá sim, sim, fazendo deploy naquele endereço.

Eu só não consigo entender se ele está colocando aqui. Então vamo, Vamos fazer o seguinte: eu vou botar mesmo esse mesmo comando, botar “--network” e vou escrever “optimism”. Agora, nesse momento eu suponho que vai rodar dentro da Optimism, então vou copiar esse endereço novamente e vou colocar aqui.

Tá? Beleza? Então o contrato criado, Como vocês podem ver, eu já estou um contrato criado, as transações estão ocorrendo aqui corretamente e o nosso contrato dele já tá fazendo o deploy dentro da Optimism. Está bom e eu acho que acredito que o básico a gente já tenha configurado, tá? O básico a gente já tem configurado e a partir dessas configurações, a partir desse repositório aqui, já com todas as dependências criadas que a gente já vai começar a poder brincar um pouco com o desenvolvimento dessa blockchain, tá?

Pessoal, então, nessa aula a gente viu alguma configuração ou setup básico no seu computador, tá? E na próxima aula a gente vai começar a adicionar e trabalhar com algumas ferramentas a mais, ok? Muito obrigado e até a próxima aula.