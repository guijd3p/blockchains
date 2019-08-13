# BlockChain

Questões DLT
1. Você é o responsável por definir qual tecnologia de DLT será utilizada para a criação de
uma rede permissionada. As únicas opões possíveis dadas as características e diretrizes
da empresa em que trabalha são R3/Corda Enterprise e Hyperledger Fabric. Com isso
em mente, que critérios (técnicos, de mercado, etc.) você utilizaria para balizar a sua
decisão entre uma ou outra? Explique os critérios.


  Para uma solução financeira vide que o solicitante em questão é a B3, uma empresa que atua no alicerce da estrutura de
capitais do Brasil, minha opção seria  pela utilização do [Corda Enterprise](https://www.r3.com/platform/), pois está 
plataforma foi idealizada e concebida para sistemas financeiros de um modo geral.
  Um [estudo](http://www.dtcc.com/news/2018/october/16/dtcc-unveils-groundbreaking-study-on-dlt) publicado pela  Depository Trust & Clearing Corporation (DTCC) 
que você poderá obter mais informações [aqui](https://medium.com/corda/throughput-a-corda-story-1bc2cb9b2b60), 
O Corda é escalável o suficiente para suportar os volumes diários do mercado acionário dos EUA, por se tratar do maior
mercado acionário do mundo, seria o suficiente para sua utilização no Brasil.
 O Hyperldger-fabric por ser mais genérico de uma forma geral, não encontrariamos estruturas internas como [financial](https://docs.corda.net/financial-model.html),
 que nós entrega uma estrutura que já seria um ótimo ponto de partida para o desenvolvimento de um [CordaApp](https://docs.corda.net/cordapp-overview.html) financeiro, 
gastando assim mais energia na soluções e regras de négocio. 
    

2. Explique quais são, na sua visão, os maiores desafios na implementação de uma rede
permissionada de DLT?

  Para implementação de uma rede Corda é necessário que exista uma entidade que administre a rede Corda, pois existe 
alguns papeis da rede como o [Networkmap]() e o [Doorman](), que são vitais para a saúde da rede Corda. Esta Entidade a
ser criada deveria administrar de forma autônoma por se tratar de um DLT todos os participantes devem compartilhar esta
responsabilidade, já sobre o Doorman existe a regulamentação no Brasil que você pode obter mais informações [aqui](https://www.iti.gov.br/acesso-a-informacao/41-lei-de-acesso-a-informacao/perguntas-frequentes/112-sobre-certificacao-digital)
no qual o Corda atualmente não tem suporte paras extenções que existe no certificado X509 utilizados pela ICP-Brasil,
para este problema deveremos realizar solicitações tanto para R3 quanto para ICP-Brasil, pois adquação desta diretrizes
nós dara segurança juridica 
  Outro desafio é difundir o conceito de que soluções deste tipo podem ser desenvolvidas em conjunto, para que o custos
e beneficios sejam para todos, não onerando apenas alguns participantes.
  

3. Você recebeu uma nova demanda de projeto com a lista de requisitos abaixo:
a. Conhecer e autorizar quem são os participantes da rede.
b. Atender a um volume de operações na ordem de grandeza de 2500 transações
por segundo.


c. Ter privacidade nos dados transacionados e armazenados, de forma que
somente os participantes que podem ver os dados da transação de fato
enxerguem e tenham acesso a esses dados.

ss voce 

d. Um Oracle ou outro tipo de fontes de dados externa irá incrementar as
transações com um índice de preço.


e. Aplicações legadas precisam ler o ledger e interagir com a rede fazendo novas
transações ou atualizações.


f. Uma tela de acompanhamento do que está rodando no Ledger precisa ser
construída.

Desenhe e explique a arquitetura da solução considerando:
a. Escolher e justificar a tecnologia entre R3/Corda Enterprise e Hyperledger
Fabric.
b. Desenho do smart contract (Cordapp ou Chaincode).
c. Desenho lógico da solução: camadas da tecnologia DLT (exemplo:
ordenação/notarização, autorização, certificação etc.), mecanismos de
integração entre os módulos e entre o Oracle e a aplicação.
d. Desenho de infraestrutura: como as camadas da tecnologia estão inseridas
numa infraestrutura corporativa incluindo firewalls, balanceadores,
datacenters etc.
e. Sizing do ambiente (quantidade de servidores e equipamentos necessários).
f. Desenho do modelo de alta disponibilidade da solução.
g. Custo aproximado da solução (pode ser baseado em informações de preços de
clouds publicas como Azure, AWS ou Google).


##Referências


https://medium.com/corda/transactions-per-second-tps-de3fb55d60e3
https://docs.corda.r3.com/sizing-and-performance.html
https://docs.corda.r3.com/performance-testing/introduction.html
https://medium.com/corda/transactions-per-second-tps-de3fb55d60e3
http://www.dtcc.com/news/2018/october/16/dtcc-unveils-groundbreaking-study-on-dlt 