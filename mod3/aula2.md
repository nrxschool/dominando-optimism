# Aula 2

Na aula anterior a gente desenvolveu o que seria nosso primeiro contrato inteligente e nessa aula a gente vai desenvolver, vai terminar de configurar o nosso nosso repo, o nosso repositório e, além disso, a gente vai desenvolver, a gente vai lidar com os nossos scripts de deploy.

Lembrando que em todo smart contract, a gente precisa desenvolver um script para que seja feito o deploy desse contrato. Ele é gente porque a gente obviamente precisa considerar qual é a chave privada, qual a wallet que vai fazer a publicação do Smart Contract. Então, nessa aula a gente vai começar a trabalhar com os nossos scripts. Então vamos aqui para tela.

Bom pessoal, então a gente tá aqui, tá no site do Optimism Faucet, tá? E como é que eu cheguei aqui? Eu vou colocar aqui na tela para vocês. Dá uma olhada então lá dentro documentação da Optimism. Eu vim aqui em Network Faucets e clique em Superchain Faucet, ok? Então vão mandar uns tokens aqui. Só que pelo que eu estou vendo, a gente precisa.

A Goerli irá depreciar, mas não vai fazer diferença.  Depois tu pode mudar pra uma outra blockchain que você quer, ok? E então tá, vamos usar a Goerli, Eu vou pedir para ele, vou pedir pro Metamesk trocar pra essa blockchain e vou pedir para ele mandar uns tokens para mim, tá? Eu não tenho nada, então vou copiar o endereço que está aqui, afinal a 13 e vou colar aqui a 13 eu vou mandar pra duas tesnets.

Coloquei os dois e claim. Vou requisitar para que me enviem os tokens falsos, ok?  Fake tokens. Se eu voltar aqui no balance e der uma olhada para ver como é que está a lá, já recebi 0,05 ETH, tá dando 112 dólares mas como eu tô dentro de uma da testnet, esse valor não tem não, não existe um valor real, tá?

É só para a gente brincar um pouquinho, ok? Então beleza, Já temos aqui 0,5. A gente já recebeu os tokens falsos para fazer o deploy dos contratos inteligentes. Então a partir de agora a gente já pode começar a brincar um pouco com os nossos contratos inteligentes, tá? E vamos criar um contrato de gente muito simples. Tá que é de pagar e receber.

Eu não sei. Eu não consigo imaginar outro contrato que seja tão simples agora. Mas sei lá, vamos criar um caixa eletrônico. Tá. Então beleza, Vamos criar um novo contrato. Vou colocar ATM.sol, só pra exemplo mesmo. Bom pessoal, então eu pedi para o ChatGPT gerar aqui um contrato ele gente, dá para a gente, é só para fins de teste. Tá aí um simple token, os events, transfer, approve e transfer from. Ele podia ter usado o ERC-20, vou pedir pra usar o ERC-20 da OpenZeppelin.

Pra usar e para usar as libraries do OpenZeppelin, a gente precisa instalar, ok? Então vamos está lá usando esse comando: “npm install @openzeppelin/contracts”

Porque o RC 20 todos esses padrões da OpenZeppelin, ele que já é uma empresa e que já fez essa auditoria, a gente pode usar com uma library, Então você vai ver que vai ser um pouquinho mais simples olha tamanho desse arquivo que a gente não tá usando o OpenZeppelin.

Agora vamos colocar e fica desse tamanho. Então, a partir desse momento, olha como é que ficou bem curtinho o nosso token. Por quê? Porque approve e  transfer e todas essas funções são nativas do ERC-20. Então você concorde se ou já tem uma função que já existe na ERC-20, só estendo pro meu contrato atual. Então, o SimpleToken está  herdando todas essas funções típicas de ERC-20.

Então agora sim a gente pode começar a fazer algumas brincadeiras e eu coloquei a ATM, né, enfim, só pra fazer um teste, ok?

Então a gente vai vim aqui em script, tá? E vou criar aqui um “deploySimpleToken.js”. E vou fazer uma cópia aqui e colar. O que aconteceu? Gente, é basicamente a mesma coisa que a gente tem aqui, tá? Só que a diferença é que a gente mudou um pouco. Eu vou corrigir, eu só tirar esses links.

É basicamente a mesma coisa, só que a gente está usando um contrato chamado Simple Token, eu já estou criando 1 milhão de tokens, certo? E aí a gente vai poder fazer o nosso deploy. Deixa eu ver, está faltando. Vamos usar a Goerli, certo? Ah, esquecemos da importação do dotenv no hardhat.config.js: “require(‘dotenv’).config”.

Vamos ver se vai rodar agora. Agora está pedindo para mudar a versão do pragma no contrato inteligente no hardhat config para 0.8.20.

Já está fazendo download do compilador 0.8.20.

Bom, ele foi, mas é assim e ele foi entre aspas porque como eu não especifiquei a network que ele criou, então ele foi na blockchain local, então não funciona muito bem do jeito que a gente quer. A gente precisa fazer o deploy desse script em uma network e qual noite que a gente vai usar? A gente vai usar o Optimism Goerli, correto?

Então mesmo comando mas adicionando a rede: “npx hardhat run scripts/deploySimpleToken.js --network optimisticGoerli”.

Também precisamos mudar a versão do solc abaixo das redes no hardhat.config.js para 0.8.20.

Não conseguiu baixar o 0.8.20.  Que estranho. Então deixa só ver o que que a gente consegue resolver aqui desse problema, então nos vemos na próxima aula.