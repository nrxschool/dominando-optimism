# Aula 2

Na aula anterior a gente utilizou o OpenZeppelin para criar o que seria o esqueleto, a estrutura no nosso padrão ERC20. Nessa aula a gente vai criar os nossos NFTs,  vai interagir com esses NFT  e vamos utilizar a OpenZeppelin para nos auxiliar a criação desse contrato. Ele é gente, Então vamos aqui para tela.

Olá pessoal! Então dessa vez a gente vai aprender sobre o que o ERC721, que são os NFTs.  Tá. Então o s ERC20 são as cryptos que a gente conhece as criptomoedas. E o padrão  ERC 721 são os são os NFTs. Então, o que a gente vai precisar testar se vamos entrar aqui na tela?

Não apenas é playing utilizando o wizard da OpenZeppelin,  a gente vai utilizar esse assistente e assistente para começar a desenvolver o nosso contrato de gente de NFT. Bom pessoal, então vão fazer uns testes novos aqui dessa vez e vão criar um em NFT. Eu quero criar, eu vou estar por esse sete dois um Fala eu quando de create a e esse é o que eu quero. “I want to transform a course intro an NFT collection, this course will be used as a reference about Optimism”  Vamos ver o que vai acontecer. Olha que interessante, ele criou um ERC-721 e olocou aqui e a possibilidade de transformar o nosso curso de Optimist num contrato inteligente. Então vamos ver que as funções que ele está iniciando a função tá, então eu tipo isso aqui. Gente, quando vocês veem essa função initialize, ele é o contructor, tá? É porque ele tá ativado aqui o upgradedable. Bom, se eu tirar esse aqui, vocês podem ver que ele voltou pro constructor, então toda vez que eu uso o upgradable, assim ele muda, ele coloca esse construct tá?

E ele coloca essa função initialize.  Bom, e então ele tem um BaseURI. Ah, então é assim. Existe várias formas da gente saber que tem várias formas de converter. A da gente transformar o nosso contrato elegante em um novo contrato.

E como vocês viram, e é, a gente pode usar o próprio chat do Wizard para criar nosso contrato inteligente por exemplo:

“Please update this smart contract to be a dragon ball z card”

Vamos ver que vai acontecer? Ele colocou aqui Dragon Ball Z e Card, então é uma collection de NFT de Dragon Ball Z.

Tá tão increase balance e essas funções abaixo são requeridas pelo Solidity. Tá? Então a gente é obrigado a usar ela, mas eles fazem um override, que que é um override é uma  re-inscrição, então ele pega o contrato e adiciona e ele reescreve função a função com novos parâmetros. Tá nesse e tá usando o upgradable, ok?

Que que o upgradable? Bom, antes de mais nada: Imagine a seguinte situação quando a gente faz o deploy de um contrato inteligente e a gente recebe um hash. É  aquele 0X32 que vai aparecer, tá? Pra vocês terem uma ideia, como é que eu posso de gerar o hash, eu vou colocar aqui “yarn hardhat run scripts/deploySimpleToken.js”

Ele subiu para esse número aqui, correto? Se eu fosse subir no novo contrato, primeiro entenda que a gente nunca pode substituir o contrato inteligente uma vez que a gente subiu para a blockchain.

Mas o que que a gente pode fazer é usar um proxy. Então, ao invés de eu ficar apontando pra um contrato inteligente e mudando o endereço contrato de gente, eu subo dois contratos, um que vai ser o pai e o outro a mãe. E não vou usar pai, mãe não, então vai ser tipo um Main e o outro é o Second.

Então o que acontece na prática é a gente sempre aponta paro Main e o Main aponta para o contrato inteligente  que a gente quiser. Então o Main vai ser isso aqui, por exemplo. Tá, eu vou até colocar embaixo, que para então o Main, pode ser isso aqui, por exemplo, coloco ali main e o second é onde está o nosso contrato inteligente.

Então vai ser contrato dele. Gente, no main  por exemplo, a gente poderia colocar e chamar isso de proxy, aí fica mais fácil. Bom, então toda vez que eu apontar para o proxy, tá algum daqui para ficar diferente? O proxy aponta para o contrato inteligente. Ah, mas eu quero subir um novo contrato, então o que que eu vou fazer?

A gente vai atualizar o novo contrato e a gente vai receber um endereço diferente, certo? Porque está fazendo novo deploy, então vai ser bla bla bla. O preencher que pode chegar até o final. Mas a gente sempre aponta o nosso sistema por proxy, porque o proxy, em vez de apontar para um como está aqui na tela, ele vai apontar para esse outro, o dois. Então ele vai apontar para um novo contrato inteligente. Então, na prática a gente usa um proxy para ter o endereço que a gente pode apontar. E esse é esse endereço. Ele serve como uma forma eu e ele é uma distribuição, ele que direciona para o contrato inteligente. Então esse é uma forma de burlar a regra de contratos da blockchain quando a gente não pode subir novos contratos, o contrato nunca muda, mas a gente pode gerar novos contratos com gente