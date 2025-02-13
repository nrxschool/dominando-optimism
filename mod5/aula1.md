# AULA 1

Então a gente, depois que a gente entendeu alguns conceitos principais de interação com o contrato inteligente, agora a gente vai entrar na parte fundamental, que é o grande diferencial da Optimism. Então, nessa aula a gente vai trabalhar de forma bem hands on. A gente vai colocar a mão na massa e criar a nossa, o nosso rollup, a camada dois na mão ou como diria como desenvolvedor, a gente vai desenvolver na unha, tá?

Então primeiramente vou fazer uma introdução e explicar para vocês o que é rollup, como funciona e depois a gente vai trabalhar com a gente, vai começar a desenvolver o nosso rollup, não é? Tá? Então vamos aqui para a tela. Agora a gente vai fazer algo muito interessante. A gente vai criar o nosso próprio rollup, tá utilizando o stack Optimism, mas a gente também vai acompanhar o Kevin Fisher que ele fez

essa apresentação tá no ETH Lisboa e aí ele faz um hands on, criando a própria solução. Esse hand-on ele tá um pouquinho desatualizado, tá? Então a gente vai fazer junto com a versão um pouquinho mais atualizada, mas a gente vai usar esse vídeo como referência, tá? Esse vídeo tem 28 minutos. Eu vou cortar algumas partes para a gente avançar nos lugares que a gente precisa e também vou fazer um paralelo aqui com a documentação atual da optimism, está?

Então vamos dar um play aqui para vocês entenderem o que eu quero dizer. Bom, esse aqui é o Kevin Fisher. Vou avançar aqui para algumas partes principais, tá? Ele pegou a documentação aqui. Essa documentação, gente, ela está desatualizada. Então é por isso que a gente vai fazer um pouco e a gente vai fazer o que eles estão propondo mas vamos fazer algumas alterações. Mas pra isso eu vou abrir essa página do Get Started ou Page Stack da Optimism. Eu vou abrir um navegador aqui no meu computador e eu vou escrever Getting Started. Bom, essa é a versão atual. Você vê que existe algumas diferenças, porque aqui ele já está dando até como se já tivesse, né?

Essa parte do Build Optimism Monorepo ele faz um clone do Optimism aqui. Se a gente for tentar adaptar, eles mudaram também, tá gente? A documentação então a gente tem que caminhar um pouco pra chegar onde a gente quer.

Bom, pessoal, consegui achar aqui, tá? Ele está dentro da parte de Builders e tutorials e a gente tem aqui o passo pra gente começar a operar. Então vamos começar com git clone. Vou voltar aqui no meu terminal. Eu só vou puxar esse terminal para cá, pro meio pra gente começar. Então vamos lá. Git Clone e Optimism. Então vamos baixar o repo do Optimism logo em seguida.

A gente precisa entrar na pasta CD Optimism. Pronto, vamos entrar. Oprtimism.

E agora a gente vai fazer o check out. Essa parte que eu não tenho certeza se tá funcionando, tá? Se eu vir aqui fazer um check out, tá. Ele tá funcionando. Então a gente fez o check out para essa parte da branch, essa branch e agora a gente vai checar nossas dependências utilizando esse comando. Então a gente tem todas as dependências aqui.

A gente pode rodar o PNP em install. Vamos dar uma avançada no vídeo. Pra que que ele fez? Tá bom, ele está fazendo o clone que a gente fez. Ele entrou na pasta. Ele está fazendo instalação igual a gente está fazendo aqui. Só que ele usou outro comando. Vocês podem ver que o comando que ele usou foi yarn install e a gente usou PNP install porque a documentação atual ela menciona isso, né? Então você vê que nesse ponto a gente já tá vendo algumas diferenças do que foi ensinado na época. Agora ele tá dando uma enrolada porque demora.

Normal, né gente? E ele faz um “make op-node op-batcher op-proposer”. Então vamos lá, vamos rodar o comando make.

Bom pessoal, terminamos aqui, agora a gente vai fazer o PNP build, correto? É mais ou menos aquele comando yarn build que ele fez. Bom pessoal, então concluímos aqui o build, vamos dar mais uma visualizada aqui no vídeo. Agora ele fez yarn build que no nosso caso foi PNP build, tá? E aqui ele faz a gente e é instruído a fazer o clone do op-geth.  Vamos ver se ele faz o mesmo.  Agora ele vai fazer o build do op-geth.

Vamos fazer isso também, mas pra isso a gente vai voltar a uma pasta anterior. Agora sim vai fazer o git clone op-geth. Depois a gente vai fazer o CD entrar na pasta e o make geth, vou fazer o CD op-geth, certo? E agora eu vou fazer o make geth, que é esse comando que está sendo instruído aqui, certo?

Agora ele fez aquele comando que a gente está fazendo, no nosso caso, em continua. Agora ele tá falando que a gente precisa do acesso ao node da Goerli, a testnet.  No nosso caso, ele pede pra ele instruir a gente, fazer uma outro mecanismo que é copiar as environment, né, pra ter essa versão do enviroment e preencher.

E aí na Layer 1, ma L1,  onde colocar, qual tipo a gente vai usar o Alchemy  e o RPC. . No nosso caso vai ser o RBC da Sepolia aqui, tá? Então a gente volta lá no Optimism.

Show de bola, Já fizemos o build e agora a gente vai votar lá na Optimism. Então vamos votar aqui e abrir dentro da parte optimism e vamos rodar o comando e cp para copiar a nossa environment, né? Vou abrir o visual code aqui tá gente?

Bom, a gente já abre o visual code, certo? Ele tá dando aqui algumas variáveis que a gente precisa necessariamente preencher e uma delas é justamente essa aqui. Então o KIND onde a gente vai usar o Alquemy e L1 kind aqui, certo? E aqui a gente vai precisar do nosso endereço da Alchemy, tá? Então eu vou colocar aqui o endereço provisório do meu RPC, tá?

Nunca compartilhe esse link. Ele é pessoal, mas no caso aqui pro fim didático eu vou copiar, mas depois eu vou exclui, tá? Então vou salvar e agora a gente vai começar a gerar os endereços admin,  batch, proposter o sequencer? Vamos rodar esse comando aqui. Ele tá dando um alerta aqui que eu não devo usar esse wallet.sh para fins de produção, tá? No nosso caso, fim didático, mas nunca rode esse comando para fins de produção, tá? Vamos gerar aqui as nossas wallets. Ele rodou, Tá, Então ele já gerou nossas wallets aqui. Eu vou copiar e vou colar dentro desse que eu achei. Se não me engano essa parte aqui mesmo tá lá.

Pronto, já tem aqui a chave privada e a chave pública novamente. Essas chaves privadas chave pública jamais compartilhem. Tá, é uma informação muito pessoal e se você tiver saldo nessas contas aqui, alguém pode roubar, tá? No meu caso não tem. Então, para fins didáticos somente a gente salvou o arquivo. Agora a gente vai fazer um fund, tá? A gente precisa enviar e ETH  para essas contas, tá que seria o admin, o proposter e o batcher. Então eu vou enviar um pouquinho desses saldos pra cada conta dessas aqui tá bom pessoal.

Bom, pra eu boter Sepolia ETH,  ou seja o token nativo da testnet da Sepolia, eu usei esse  Alchemy Faucet. Então eu ganho 0,5 sepolia  e eu preciso colocar necessariamente a chave pública. Eu mandei para uma chave pública que eu uso para fim de desenvolvimento e depois eu reenviei pras outras contas. Você pode ver que aqui ele gerou o seguinte e mandou para minha carteira. Depois eu fiz a redistribuição.

Então eu coloquei ETH sepolia nativo para essas contas aqui, conforme ele pede para a gente mandar. Só que eu mandei só 0,1 Tá gente, eu não mudei muito mais que isso não. Se deu algum erro, a gente sabe, tá? Agora a gente vai voltar lá na Optimism. Já estamos né, a gente vai fazer e rodar esse comando aqui, eu vou limpar aqui e vou dar o comando.

Pronto. Pessoal, no meu caso a gente se você viu que não deu certo, quando eu coloquei esse comando aqui, que eu tive que fazer, eu tive que rodar esse comando aqui antes, tá? Que vocês estão vendo aqui na tela. E aí agora sim eu consigo liberar né? As variáveis de ambiente vou dar um clear aqui e vão continuar aqui o nosso tutorial.

Agora a gente vai rodar esse comando aqui tá? A gente vai tá dentro da Optimism, dentro do contracts-bedrock, tá assim e vão mudar esse comando aqui de config. Rodei ele tá falando aqui que a gente pode abrir esse arquivo para ver se está tudo certo. Vou fazer um get que para ver. E tem coisa aqui dentro tem conteúdo e o arquivo existe. Essa parte aqui é opcional. Se a gente tiver fazendo uma chain além da Sepolia a gente pode criar esse create2 Factory. E enfim, é algo. Vamos pular por enquanto, tá? Então vamos rodar esse comando aqui, tá deploy the L1 contracts. Vou copiar e vou rodar o script. Deixa um clear  aqui. A gente teve um erro aqui, provavelmente uma das nossas contas não tinha, não teve o saldo suficiente, então a gente vai ter que eu rodei que que colocar mais saldo, tá?

E eu só mandei 0,1 ETH. Eu só preciso ver qual a conta que não deu certo ou vou mandar para todas elas. Não vai ter jeito. Vou mandar mais um pouquinho de saldo aqui, refazer esse comando. Bom, mandem mais um pouquinho de dinheiro, vamos testar de novo e esse comando.