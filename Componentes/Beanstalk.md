<h2 align="center"> AWS Elastic Beanstalk </h2>

<div align="justify">
<p>AWS Elastic Beanstalk é um serviço da AWS que permite que os programadores e engenheiros possam facilmente implementar e executar aplicações web na cloud, de uma forma que seja altamente disponível e escalável.</p>  

<p>Este serviço da AWS trata da parte da implementação, provisionamento, monitorização, escalabilidade automática e gestão da nossa aplicação. Em termos de implementação, podemos fazer upload e gerir diferentes versões da aplicação, e mudar entre elas em ambientes diferentes (por exemplo, desenvolvimento, teste, ambientes de produção). Além disso, quando implementamos a nossa aplicação, o Elastic Beanstalk provisiona as instâncias necessárias, em termos de capacidade de computação, os load balancers, auto-scaling e recursos de monitorização do funcionamento das nossas aplicações. Este último ponto é bastante importante, dado que quando temos a nossa aplicação a correr em produção, o Beanstalk faz verificações regulares de funcionamento das aplicações, de forma a garantir que a mesma está a correr, sendo que se não estiver, irá tentar encontrar o erro e resolvê-lo. Podemos, também, ter acesso às métricas de monitorização do Amazon CloudWatch (contagem de pedidos, uso do CPU, entre outros).</p>    


<h3 align="center"> Componentes do Elastic Beanstalk </h3>

O Elastic Beanstalk possuí vários componentes essenciais, sendo eles: 
<ul>
  <li>Versão da Aplicação</li>
</ul>

Versão da aplicação refere-se à aplicação web que carregou e irá carregar a sua próxima versão atualizada. Por exemplo, primeiro faz-se o upload da aplicação para AWS Beanstalk e depois atualiza-se o código fonte da aplicação. Em vez de escrever por cima da versão anterior da aplicação, pode-se dar-lhe um novo nome de versão que poderá ser utilizado para comparar ambas. A versão nomeada aparecerá como uma nova aplicação caso opte-se por implementá-la num ambiente diferente em vez de a implementar a partir de uma aplicação existente. No Elastic Beanstalk, a versão da aplicação é uma ligação a um objeto AWS S3 (Simple Storage Service) que contém o ficheiro Zip ou Java WAR implementado.  

<ul>
  <li>Aplicação</li>
</ul>
 
Uma aplicação no Beanstalk é uma coleção de ambientes, versões e eventos. No AWS Elastic Beanstalk, carrega-se a aplicação como um ficheiro zip com todo o conteúdo nela contido. Uma aplicação Elastic Beanstalk é logicamente considerada equivalente a um ficheiro contendo o código fonte. O ficheiro é a aplicação no ambiente do Elastic Beanstalk. Normalmente, pode-se criar uma aplicação para cada uma das aplicações, mas isto não é necessário. 

<ul>
  <li>Ambientes</li>
</ul>

Um ambiente tem uma versão implementada em instâncias específicas, load balancers, grupos de auto-scaling, entre outros. Pode-se implementar uma das versões existentes em qualquer ambiente dentro da aplicação. Tipicamente, poder-se-ia criar um ambiente para a produção e outro para testes, contudo pode-se criar os ambientes que precisamos. Um ambiente pode estar em diferentes estados de saúde: verde (OK), amarelo (não respondeu nos últimos 5 minutos), vermelho (não responde há mais de 5 minutos), cinzento (desconhecido). Sempre que é criado um ambiente, a Amazon Elastic Beanstalk provisiona automaticamente as instâncias EC2 e os S3 buckets. 

<ul>
  <li>Nível de ambiente</li>
</ul>

Existem dois níveis de ambiente quando implementamos uma aplicação no Beanstalk: Ambiente do Servidor Web e Ambiente do Trabalhador. Uma aplicação que utiliza PHP ou requer pedidos HTTP é executada num Ambiente de Servidor Web. Uma aplicação que utiliza Amazon Simple Queue Service (SQS) é executada num Ambiente de Trabalho. 

<ul>
  <li>Configuração do ambiente</li>
</ul>

A configuração do ambiente é um conjunto de parâmetros como o grupo de segurança, o tipo de instância e a versão de plataforma. Se se alterar alguma configuração, o Amazon Elastic Beanstalk implementa-a de forma dinâmica, aplicando as novas alterações ou apagado e implementando novos recursos. 

<ul>
  <li>Eventos</li>
</ul>

Os eventos dizem aos utilizadores o que se está a passar com os seus ambientes. Podem ser informativos, avisos ou erros, tais como "o ambiente foi lançado de forma bem-sucedida", "a instância X está a usar 90% do CPU" ou "a instância X não iniciou corretamente". Pode-se ver os eventos na web console ou pode-se obtê-los por e-mail. 

<ul>
  <li>Plataforma</li>
</ul>

A plataforma é a combinação de todos os componentes do AWS Beanstalk, um sistema operativo, runtime de uma linguagem de programação e um servidor web para correr a aplicação. Pode-se escolher a plataforma enquanto se cria a aplicação ou ambiente, sendo que não precisamos de a atualizar ou incluir correções de software, a AWS encarrega-se disso.  

<h3 align="center">Vantagens</h3>
  
<ul>
  <li>Preço acessível - O Beanstalk proporciona aos seus utilizadores infraestruturas de baixo custo, ou seja, paga-se apenas pelo que se usa e não há taxas escondidas.</li>
  <li>Acesso Rápido - Através da AWS Management Console, é possível ter acesso à plataforma em menos de uma hora. </li>
  <li>Fácil acesso à automatização - para a maioria dos clientes, este é o principal benefício do Beanstalk: é possível fazer o setup da infraestrutura com pouco input por parte do utilizador. 
</li>
  <li>Custo – O Beanstalk não tem custos adicionais, apenas é necessário pagar pelos recursos que este disponibiliza. </li>
  <li>Flexibilidade - é possível gerir manualmente qualquer aspeto dos recursos proporcionados pelo Beanstalk. </li>
</ul>

<h3 align="center">Desvantagens</h3>
  
<ul>
  <li>Não é fácil diagnosticar falhas – O Beanstalk ao gerir tudo automaticamente, torna difícil determinar exatamente onde este errou. </li>
  <li>Deployment lento – Por vezes o provisionamento das instâncias pode ser delongado, podendo demorar entre 5 e 15 minutos.</li>
  <li>Updates da stack – Devido à sua natureza automática o Beanstalk efetua as modificações necessárias aos recursos alocados através de atualizações, o que por vezes pode causar problemas, no entanto na maioria dos casos será completamente inofensivo. </li>
  <li>Falta de controlo detalhado – Embora existam muitas configurações padrão disponibilizadas para um projeto Beanstalk, é possível que existam casos de utilização para os quais não exista uma configuração adequada.</li>
</ul>
  
</div>
