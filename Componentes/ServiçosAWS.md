<h2 align="center"> Outros Serviços AWS </h2>

<div align="justify">
<br>
<p><b>AWS Code Deploy</b></p>

<p>CodeDeploy é um serviço fornecido pela AWS que automatiza a implementação de software para uma variedade de serviços informáticos, eliminando assim a necessidade de uma implementação manual propensa a erros. Este serviço pode ser utilizado para implementar qualquer tipo de aplicação, sendo que nesta plataforma determinam-se os ficheiros a copiar e os scripts a executar em cada instância durante o desdobramento <a href="https://aws.amazon.com/pt/codedeploy/faqs"> [12]</a>.</p>
  
  
<div align="center">
<img src="https://user-images.githubusercontent.com/102309065/160596206-000a8f11-d67c-4727-8942-c87ddac0d140.png">
</div>

<p>O AWS CodeDeploy foi concebido essencialmente para programadores e administradores que necessitem de implementar aplicações em qualquer instancia, sendo que este serviço facilita um deployment rápido de novas funcionalidades, evita paragens durante a implementação de aplicações, trata as atualizações de forma automática e escala-se de forma a responder às necessidades do utilizador <a href="https://aws.amazon.com/pt/codedeploy"> [13]</a>. </p>
  
<div align="center">  
<img src="https://user-images.githubusercontent.com/102309065/160596216-744de092-2bb7-4ce6-8f48-449458190282.png">
</div>

<p>O AWS CodeDeploy é independente de qualquer linguagem de programação e possui uma arquitetura agnóstica, ou seja é possível utilizar scripts para qualquer lógica de implementação personalizada.</p>

<p>O que diferencia o AWS CodeDeploy do AWS Elastic Beanstalk é o facto do Beanstalk ser uma solução de gestão de apilcações ponta-a-ponta enquanto que o AWS CodeDeploy é um serviço de blocos de construção centralizado em ajudar os programadores a implementar e atualizar software em qualquer instância <a href="https://aws.amazon.com/pt/codedeploy/faqs"> [12]</a>. </p>

<br>
  <p><b>AWS Code Pipeline</b></p>

<p>AWS CodePipeline é um serviço que automatiza o processo de implementação de software, permitindo ao programador modelar, visualizar e fornecer rapidamente o código para novas funcionalidades e actualizações. Assim, o programador consegue aumentar a velocidade e a qualidade das suas actualizações de software, executando todas as novas alterações através de um conjunto coeso de verificações de qualidade. Com este serviço o pagamento é feito apenas pelo utilizado, não havendo taxas iniciais ou compromissos a longo prazo <a href="https://aws.amazon.com/codepipeline/?nc=sn&loc=0"> [14]</a> <a href="https://aws.amazon.com/codepipeline/faqs/?nc1=h_ls"> [15]</a>. </p>

<p>De uma forma geral, com o AWS CodePipeline é possível modelar, o processo completo de lançamento e teste de uma aplicação e sua a implementação em ambientes de pré-produção. O serviço constrói, testa e implementa a aplicação de acordo com o modelo de lançamento definido pelo programador, sempre que há uma alteração de código <a href="https://aws.amazon.com/codepipeline/faqs/?nc1=h_ls"> [15]</a>. </p>

<p>O AWS CodePipeline pode também ser integrado facilmente com serviços de terceiros como o GitHub ou com plugin personalizado do utilizador <a href="https://aws.amazon.com/codepipeline/faqs/?nc1=h_ls"> [15]</a>.</p>

<p>O CodeDeploy difere do AWS Elastic Beanstalk pois, enquanto que o Beanstalk tenta simplificar a gestão de recursos fazendo-o pelo programador, com o CodeDeploy o programador necessita de criar a sua própria infraestrutura tendo assim controlo total sobre esses recursos <a href="https://aws.amazon.com/codepipeline/faqs/?nc1=h_ls"> [15]</a>.</p>

![product-page-diagram_CodePipeLine 7b8dd19eb6478b7f6f747d936c2f0b0b66757bbf](https://user-images.githubusercontent.com/102309065/160596428-55feafce-3f2f-4530-b5e4-2803465bb3f9.png)
<br>
<br>
<p><b>AWS CodeStar</b></p>

<p>AWS CodeStar é um serviço de desenvolvimento baseado na nuvem que disponibiliza ao utilizador ferramentas necessárias para desenvolver, construir e implementar rapidamente aplicações no AWS, oferecendo essencialmente uma interface de utilizador unificada que permite uma fácil gestão das atividades de desenvolvimento de software num só local. Com este serviço não existe nenhum custo adicional pela utilização, sendo que o utilizador paga apenas pelos recursos disponibilizados pela AWS para o desenvolvimento e execução da sua aplicação <a href="https://aws.amazon.com/codestar/faqs/?nc=sn&loc=4"> [16]</a> <a href="https://aws.amazon.com/codestar/?nc=sn&loc=0"> [17]</a>.  </p>

<p>Com o AWS CodeStar é possível configurar toda a sua cadeia de ferramentas de entrega contínua em minutos o que por sua vez, permite começar a lançar o código mais rapidamente.</p>

<p>O AWS CodeStar facilita o trabalho em equipa de forma segura, com políticas integradas que permitem uma fácil gestão do acesso e adição de proprietários, contribuidores e espectadores aos projetos.</p> 

<p>No fundo, o AWS CodeStar facilita a configuração de toda a cadeia de ferramentas de desenvolvimento e entrega de modo a simplificar a construção, testagem e implementação do código de aplicação, este auxilia a coordenação das suas atividades diárias de desenvolvimento através de um painel unificado de projetos o que por sua vez, permite monitorizar a atividade da aplicação, e acompanhar o progresso em todas as fases do seu processo de desenvolvimento <a href="https://aws.amazon.com/codestar/faqs/?nc=sn&loc=4"> [16]</a> <a href="https://aws.amazon.com/codestar/?nc=sn&loc=0"> [17]</a>. </p>

<p>Ao analisar tanto o CodeStar como o BeanStalk torna-se evidente que o CodeStar, engloba tanto os serviços de deployment e testagem de código (Code Pipeline) como as múltiplas possibilidades de provisionamento de infraestrutura, sendo que quando se configura o CodeStar para além das opções de Amazon EC2 ou Lambda, que são de configuração mais complexa, também é possível optar pela utilização do Elastic Beanstalk de modo a simplificar o processo <a href="https://aws.amazon.com/codestar/faqs/?nc=sn&loc=4"> [16]</a> <a href="https://aws.amazon.com/codestar/?nc=sn&loc=0"> [17]</a>.  </p>
 
  <div align="center">
<img src="https://user-images.githubusercontent.com/102309065/160596568-120f6580-3dce-449c-b6e0-348ae9ba3b72.png">
  </div>
 </div>
 
<br>
<div align="center">
<p>Anterior: <a href="https://github.com/MrBen777/Trabalho_PaaS_Grupo_4/blob/main/Componentes/Competidores.md">Competidores<a> | Próximo: <a href="https://github.com/MrBen777/Trabalho_PaaS_Grupo_4/blob/main/Componentes/CasosDeEstudo.md">Casos de Estudo</a></p>
<p><a href="https://github.com/MrBen777/Trabalho_PaaS_Grupo_4/blob/main/README.md">Página Principal</a></p>
<p><a href="https://github.com/MrBen777/Trabalho_PaaS_Grupo_4/blob/main/Componentes/Bibliografia.md">Bibliografia<a></p>
</div>

