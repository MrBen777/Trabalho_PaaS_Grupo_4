<h2 align="center"> AWS Elastic Beanstalk </h2>
<br>

<div align="justify">
<p>O AWS Elastic Beanstalk é um serviço da AWS que permite a que developers possam implementar e executar aplicações na cloud com facilidade, de uma forma que seja altamente disponível e escalável.</p>  

<p>Este serviço da AWS facilita ao utilizador toda a parte da implementação, provisionamento de recursos, monitorização, escalabilidade e gestão da aplicação. Em termos de implementação, podemos fazer upload e gerir diferentes versões da aplicação, sendo possível optar entre a utilização de versões diferentes consoante a necessidade do cliente (por exemplo poderia ser possível escolher entre versões em desenvolvimento, ou para teste). Resumidamente, quando implementamos a nossa aplicação, o Elastic Beanstalk aloca-lhe as instâncias necessárias, tanto em termos de capacidade como de computação, dando também uso a load balancers de modo a gerir o tráfego que lhe é necessário [2].</p>  
  
<p>Podemos, também, ter acesso à monitorização de várias métricas relevantes à infraestrutura que nos foi alocada pela plataforma através do Amazon CloudWatch (contagem de pedidos, uso do CPU, entre outros). Para além de todos estes recursos disponibilizados também é facilitada ao utilizador, uma plataforma de monitorização do funcionamento das aplicações. Este último ponto é bastante importante, dado que quando se corre aplicações em produção, o Beanstalk faz verificações regulares sobre funcionamento destas, de forma a garantir que as aplicações estão de facto a ser executadas, sendo que em caso contrário, irá tentar encontrar o erro e resolvê-lo [2].</p>  

<br>
<h3> Componentes do Elastic Beanstalk </h3>
<br>

O Elastic Beanstalk possuí vários componentes essenciais, sendo eles: 
<ul>
  <b><li>Versão da Aplicação</li></b>
</ul>

<p>Quando subscrevemos a um serviço de Elastic Beanstalk é requerido ao utilizador que este forneça em primeira instância, a aplicação, criada previamente, da qual se pretende fazer a implementação/deployment, sendo que posteriormente é possível criar versões novas desta de modo a proceder a atualizações ou caso seja necessário, executar a aplicação dentro de um ambiente de testes [2].</p> 

  <div align="center">
  <img src="https://user-images.githubusercontent.com/91042645/160619001-c3fac283-f147-4355-bbbb-bcf70e0df27a.PNG">
  </div>
  
<p>Como exemplificado na figura acima, este processo de criação de versões pode ser compreendido, como algo a realizar iterativamente, sendo que também é possível ao cliente não rescrever a versão anterior da aplicação podendo então optar por dar-lhe um novo nome, sendo que a posteriori lhe será possível comparar ambas as versões. A versão alternativa aparecerá como uma nova aplicação caso se opte por implementá-la num ambiente diferente.</p>  

<ul>
<b><li>Aplicação</li></b>
</ul>
 
<p>Uma aplicação no Beanstalk é uma coleção de ambientes, versões e eventos. No AWS Elastic Beanstalk, carrega-se a aplicação como um ficheiro zip com todo o conteúdo nela contido. Uma aplicação Elastic Beanstalk é logicamente considerada equivalente a um ficheiro contendo o código fonte. O ficheiro é a aplicação no ambiente do Elastic Beanstalk. Normalmente, pode-se criar uma aplicação para cada uma das aplicações, mas isto não é necessário [3].</p> 

<ul>
<b><li>Ambientes</li></b>
</ul>

<p>Um ambiente tem uma versão implementada em instâncias específicas, load balancers, grupos de auto-scaling, entre outros. Pode-se implementar uma das versões existentes em qualquer ambiente dentro da aplicação. Tipicamente, poder-se-ia criar um ambiente para a produção e outro para testes, contudo pode-se criar os ambientes que precisamos. Um ambiente pode estar em diferentes estados de saúde: verde (OK), amarelo (não respondeu nos últimos 5 minutos), vermelho (não responde há mais de 5 minutos), cinzento (desconhecido). Sempre que é criado um ambiente, a Amazon Elastic Beanstalk provisiona automaticamente as instâncias EC2 e os S3 buckets [2].</p> 

<ul>
<b><li>Nível de ambiente</li></b>
</ul>

<p>Existem dois níveis de ambiente quando implementamos uma aplicação no Beanstalk: Ambiente do Servidor Web e Ambiente do Trabalhador. Uma aplicação que utiliza PHP ou requer pedidos HTTP é executada num Ambiente de Servidor Web. Uma aplicação que utiliza Amazon Simple Queue Service (SQS) é executada num Ambiente de Trabalho [3].</p> 

<ul>
 <b><li>Configuração do ambiente</li></b>
</ul>

<p>A configuração do ambiente é um conjunto de parâmetros como o grupo de segurança, o tipo de instância e a versão de plataforma. Se se alterar alguma configuração, o Amazon Elastic Beanstalk implementa-a de forma dinâmica, aplicando as novas alterações ou apagado e implementando novos recursos [3].</p> 

<ul>
<b><li>Eventos</li></b>
</ul>

<p>Os eventos dizem aos utilizadores o que se está a passar com os seus ambientes. Podem ser informativos, avisos ou erros, tais como "o ambiente foi lançado de forma bem-sucedida", "a instância X está a usar 90% do CPU" ou "a instância X não iniciou corretamente". Pode-se ver os eventos na web console ou pode-se obtê-los por e-mail [2].</p> 

<ul>
<b><li>Plataforma</li></b>
</ul>

<p>A plataforma é a combinação de todos os componentes do AWS Beanstalk, um sistema operativo, runtime de uma linguagem de programação e um servidor web para correr a aplicação. Pode-se escolher a plataforma enquanto se cria a aplicação ou ambiente, sendo que não precisamos de a atualizar ou incluir correções de software, a AWS encarrega-se disso [3].</p> 
<br>
<h3> Funcionamento do Elastic Beanstalk </h3>
<br>
  
Antes de utilizar o Amazon Elastic Beanstalk, é necessário criar uma aplicação local em qualquer plataforma, por exemplo Java, .NET, PHP, Node.js, Python, Ruby, Go,Docker, entre outros. Depois disso, tem de se criar uma aplicação em Elastic Beanstalk com um ambiente onde possa carregar a aplicação local. Em seguida, implementá-la e utilizar a URL fornecido para a lançar. 

Não há custos aplicados ao Elastic Beanstalk no AWS separadamente, apenas paga-se pelos recursos que se utiliza para executar a aplicação. Além disso, o custo não é fixo, pode variar com o número de instâncias EC2, tamanho do bucket S3 e a configuração das instâncias da database [3].  
  
<br>
<h3>Vantagens [4][5]</h3>
  
<ul>
  <li>Preço acessível - O Beanstalk proporciona aos seus utilizadores infraestruturas de baixo custo, ou seja, paga-se apenas pelo que se usa e não há taxas escondidas.</li>
  <li>Acesso Rápido - Através da AWS Management Console, é possível ter acesso à plataforma em menos de uma hora. </li>
  <li>Fácil acesso à automatização - para a maioria dos clientes, este é o principal benefício do Beanstalk: é possível fazer o setup da infraestrutura com pouco input por parte do utilizador. 
</li>
  <li>Custo – O Beanstalk não tem custos adicionais, apenas é necessário pagar pelos recursos que este disponibiliza. </li>
  <li>Flexibilidade - é possível gerir manualmente qualquer aspeto dos recursos proporcionados pelo Beanstalk. </li>
</ul>
<br>
<h3>Desvantagens [4][5]</h3>
  
<ul>
  <li>Não é fácil diagnosticar falhas – O Beanstalk ao gerir tudo automaticamente, torna difícil determinar exatamente onde este errou. </li>
  <li>Deployment lento – Por vezes o provisionamento das instâncias pode ser delongado, podendo demorar entre 5 e 15 minutos.</li>
  <li>Updates da stack – Devido à sua natureza automática o Beanstalk efetua as modificações necessárias aos recursos alocados através de atualizações, o que por vezes pode causar problemas, no entanto na maioria dos casos será completamente inofensivo. </li>
  <li>Falta de controlo detalhado – Embora existam muitas configurações padrão disponibilizadas para um projeto Beanstalk, é possível que existam casos de utilização para os quais não exista uma configuração adequada.</li>
</ul>
  
</div>
