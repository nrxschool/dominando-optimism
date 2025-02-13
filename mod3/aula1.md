# Aula 1

Então, nessa aula a gente vai começar a desenvolver o que seria o nosso primeiro contrato inteligente. Então a gente vai além de configurar o nosso Hardhart que a gente aprendeu na  aula passada e agora a gente vai começar a colocar em ação nossos primeiros contratos inteligentes. Então vão aqui pra tela, vão. Vão começar a configurar o nosso primeiro contrato inteligente, o nosso primeiro repo com um contrato inteligente.

Então, para isso eu vou. Eu vou entrar dentro de um diretório aqui no meu computador e vou chamar esse projeto. Eu posso fazer o seguinte deixa eu só ver que eu comando. Bom pessoal, então eu vou criar aqui um diretório chamado e eu vou colocar o comando mkdir para criar uma pasta e eu vou criar o nome de e vou colocar esse nome aqui Optimism Hardhat Project.

E vou dar um CD, tá? CD Optimism e entrei dentro da pasta, tá? Essa pasta está vazia, está a gente se der um LS que está vazia, então como é que eu faço para iniciar um novo projeto da do Hardhat E eu uso esse comando aqui, o NPX Hardhat. Gente, o que eu estou considerando aqui tá que vocês já tem instalado o NodeJS, tá?

Se eu apertar o botãozinho aqui, não, o de trás se interessa. Em version eu estou na versão 20,7, então o meu NodeJS já está instalado. Então eu consigo..  eu não sei se tem NPX version desta forma. Tem. Então eu também tenho instalado NPX. Então vou considerar que vocês já instalaram o Node e também o Hardhat. Tá. Então vamos lá.

Tá, você pode. Você também pode estar lá dessa forma. Aqui você pode digitar o comando. Se você não tiver instalado, você pode botar “npm install global hardhat”, dessa forma. Mas eu já tem instalado aqui. Vou colocar o comando NPX  hardhat, tá? Que que eu estou fazendo nesse momento? Eu estou iniciando e Wizard do hardhat tá?

E eu vou trazer alguns repos,  eu vou construir a estrutura do meu projeto baseado numa estrutura padrão do hardhat. Eu poderia escolher esse Typescript,  Javascript. Eu nesse momento eu vou botar só JavaScript. Eu gosto de sempre usar esse projeto padrão, tá? Eu vou apertar Yes, vou adicionar o gitignore.  Vou instalar dependências e pronto.

Agora vamos aguardar a instalação aí do nosso repositório.

Prontinho pessoal! Então foi instalado ele aparece esse essa mensagem. Se eu der aqui um LS vou ver alguns arquivos que foram gerados, certo? E aí, o que que a gente pode fazer? Pra a gente já deixar tudo configurado, a gente pode rodar o comando “npm install @eth-optimism/hardhat-ovm”. Então a gente vai instalar a library da Optimism no nosso repo, que até então era simplesmente um projeto hardhat comum. E agora que a gente vai começar a adaptar para o nosso ambiente da Optimism, ok? Bom, dito isso, o que que eu fiz aqui?

Eu escrevi code espaço ponto. Tá, significa que eu vou abrir o Visual Code  no diretório atual. E aqui está o nosso projeto que é interessante. Então nós temos aqui alguns contratos. Isso aqui é um contrato padrão. Bom, se eu vier aqui colocar “npx hardhat test test/Lock.js” E aí ele vai testar o nosso, o nosso help por padrão.

Então o que eu fiz? Eu rodei o comando e eu fiz o start desse arquivo .js, o Lock.js. A gente não escreveu nada que foi gerado com nosso script de de geração de arquivos, tá?

Então nada aqui a gente escreveu, a gente nem vai precisar, na verdade, disso, mas vamos deixar, porque para mim é útil. Quando eu quero criar um arquivo novo, aí eu tenho uma referência já. Bom, o que a gente precisa adaptar aqui também. Certo? A gente também precisa adaptar o nosso hardhat pra usar a blockchain da Optimism.

Outra coisa que a gente vai fazer aqui, pessoal, é instalar o dotenv. “Npm install dotenv”. O que é esse dotenv?  Quando a gente lida com variáveis de ambiente — o que é uma variável de ambiente? Geralmente é uma variável que a gente configura, que fica lá criptografada, escondidinha, mas ela só existe naquele ambiente. E aí, nesse caso, a gente pode fazer isso criando um novo arquivo chamado .env dessa forma.

E aí a gente pode escrever várias variáveis, a gente pode criar várias variáveis aqui, como testnet é igual a isso, então lá no servidor essa informação pode ser uma e etc etc. Ok, então vamos lá. Eu já instalei o dotenv. Agora eu vou dar uma configurada aqui no nosso hardhat config, tá? Se eu vier aqui e colar o que que eu tenho aqui na minha tela?

Vamos lá. Eu tenho aqui algumas testnets que é a Kovan e da Goerli. Com gsas price, que aqui é um valor padrão, tá gente, aqui eu extrai do ChatGPT e aqui tem aqui o endpoint da mainnet, tá? E outras fontes de testnets, ok? Bom, que informação que a gente vai precisar aqui é dessa private key. Então no ambiente de vocês, vocês vão criar dentro do arquivo .env, vocês colocam “PRIVATE_KEY=” e coloque aí a private keyy com que vocês querem trabalhar. No meu caso eu tenho várias private key  e obviamente nunca recomendo vocês dividirem de nenhuma forma private key. Se alguém tem acesso para ver que até e tiver valor de lá, você provavelmente vai perder, porque essa pessoa pode acessar.

Então, acostumem-se a não compartilhar a private key. A private key que eu vou colocar aqui não tem nenhum valor, não tem nenhum token lá, eu sou somente para fins didáticos.Então eu vou colar aqui, certo? É isso aqui, a prrivate key  da minha account que eu vou trabalhar.

Então o que acontece? Agora eu configurei para que qualquer teste ou deploy de smart contract que eu faça na rede da Optimism, eu vou usar a minha private key  que está dentro desse array, um array único. Poderia até que colocar outras keys aqui também, ok, mas eu vou usar a minha private key. Então, quando vocês leem esse .env, significa que ele vai ler a variável que está armazenada aqui.

Então o que que ele vai fazer? Ele vai fazer o deploy, teste, qualquer outra coisa que envolva uma wallet usando a private key que a gente configurou lá, certo?

Bom, dito isso, nós temos configurado aqui algumas coisas e eu acredito que a gente possa fazer alguns testes. Eu vou precisar pegar um faucet e mandar alguns tokens falsos, fake  tokens para minha conta, ok?

Então na próxima aula a gente vai fazer isso junto. Então se você chegou até aqui, você já configurou alguns endpoints dentro do seu repo do hardhat. Tem o package.json, outras coisas aqui e um contrato. Todos os arquivos foram gerados automaticamente, ok? Então nos vemos na próxima aula pessoal.