<h2 align="center"> Casos de Estudo </h2>
<br>
<h3>Zillow</h3> 

<div align="justify">

<p>A Zillow, criada por Rich Barton e Lloyd Frink, ex-executivos da Microsoft, é uma empresa americana, fundada em 2004, cujo principal serviço baseia-se num marketplace de imobiliário online. A Zillow processa uma quantidade enorme de imagens novas diariamente, desde fotos de listagem a imagens de possíveis projetos de casa <a href="https://en.wikipedia.org/wiki/Zillow"> [18]</a>. </p>

<p>À medida que a empresa aumentou em popularidade e as imagens introduzidas no website começaram a aumentar em resolução, o sistema tradicional de processamento de imagens da Zillow não conseguiu acompanhar a procura. O sistema era alojado em datacenters On-Premisses e as imagens em si eram fornecidas a uma rede de entrega de conteúdos (CDN) através de uma queue singular. Este sistema era dispendioso e não era eficiente o suficiente para conseguir lidar com a quantidade massiva de requests diários.</p>

<p>A Zillow também sofria de dificuldades com a performance do seu sistema de processamento de imagens. O ritmo elevado a que novas imagens entravam no sistema aliado a possíveis variações na velocidade de acesso às imagens, a partir de certas fontes, causava a existência da possibilidade de que uma imagem atrasada no topo da queue pudesse impedir que as imagens subsequentes fossem descarregadas.</p>

<p>A solução para estes problemas baseia-se na escolha de uma arquitetura baseada na cloud que visa resolver os problemas de escalabilidade e desempenho do sistema de imagens. Optando por usar instâncias da Amazon Elastic Compute Cloud (Amazon EC2) e Amazon Simple Storage Service (Amazon S3) para o armazenamento das imagens, a Zillow migrou o alojamento e distribuição de imagens de uma instalação On-Premisses para a cloud da AWS.</p>

<p>O AWS Elastic Beanstalk foi utilizado pela Zillow como um meio para criar e fornecer um ambiente de trabalho onde foi desenvolvida uma biblioteca de imagens em Python, capaz de executar código customizado. Devido às variações na necessidade de capacidade de ingestão de imagens, era necessário um sistema altamente escalável, consoante o necessário, sendo que o Elastic Beanstalk era a opção mais simples de o conseguir.</p>

<p>Graças aos serviços da AWS a preocupação com a capacidade dos seus sistemas deixa de ser necessária. A Zillow agora possui a escalabilidade e o desempenho necessário para exibir aos seus utilizadores imagens de alta qualidade, algo fundamental para a uma experiência de utilizador de qualidade. O download e processamento de imagens pode ser escalado, de modo a atender a diferentes volumes de imagens recebidas ao longo do dia <a href="https://aws.amazon.com/solutions/case-studies/zillow"> [19]</a>.</p>

<h3>Ividata</h3> 
 
<p>A Ividata é uma empresa de consultoria especializada em Big Data, com sede em Paris, fundada no final de 2013. Focando-se na inovação e investindo em investigação e desenvolvimento, a Ividata criou uma solução de análise de retalho chamada Ivizone que fornece aos comerciantes uma página web acessível por wi-fi, através da qual podem melhorar os seus esforços de marketing e apresentar ofertas altamente direcionadas aos seus consumidores. Para além do mencionado esta ferramenta também permite fazer o rastreio de vários dados, tal como; a contagem de visitantes, a duração de cada visita e o tráfico pedonal dentro e nas proximidades das lojas.</p> 

<p>A infraestrutura da Ividata foi inicialmente alimentada por uma série de serviços PaaS providenciados através de diversos fornecedores. Ao utilizar estes serviços a empresa conseguiu iniciar a produção do Ivizone rapidamente. As vantagens de poder iniciar desenvolvimento dos seus produtos tão rapidamente numa fase tão precoce como uma empresa eram enormes.</p> 

<p>Rapidamente, a Ividata confrontou-se com despesas crescentes e problemas relativos ao processamento de dados. Estes obstáculos estavam a impor restrições à sua rápida expansão. De modo a manter o mesmo ritmo de desenvolvimento e evolução, era necessária uma infraestrutura reativa e escalável que permitisse fornecer serviços de qualidade aos clientes.</p> 

<p>Dados os problemas com as suas infraestruturas anteriores, a decisão de migração baseou-se na escolha de um fornecedor que possibilitasse a melhor relação custo-eficácia, assim sendo a Ividata optou pela AWS, pois sabia que não iria ter problemas de escalabilidade ou custos.</p>  

<p>Recorrendo aos vários serviços oferecidos pela AWS a implementação passa por adquirir os dados de localização dos smartphones dos clientes, através da rede wi-fi, que por sua vez é ingerida por um servidor hospedado no AWS Elastic Beanstalk. A Ividata também utiliza Elastic Load Balancing para gerir o tráfego entre instâncias (EC2) que estão espalhadas por multiplas zonas de disponibilidade. Ou seja, se houver algum problema num datacenter, os sistemas mantêm-se online.</p>  

<p>A posteriori, os registos da análise dos dados são escritos para servidores da Amazon Kinesis, agregados e comprimidos através da Amazon Kinesis Client Library (KCL) e a AWS Kinesis Connector Library, armazenados no Amazon Simple Storage Service (Amazon S3) e avaliados em tempo real através do Amazon Elastic MapReduce (Amazon EMR), antes de serem colocados numa base de dados (Amazon RDS).</p>  

<p>A relação custo-eficácia dos serviços de TI é crítica para todas as empresas que trabalham em mercados acelerados. A Ividata desde que migrou para a AWS tem visto um aumento na agilidade operacional e poupança, relativamente aos custos.</p>  

<p>Os servidores da Ividata, configurados através do AWS Elastic Beanstalk, são cerca de quatro vezes mais rentáveis do que a soluções de PaaS utilizadas anteriormente, o que teve um impacto importante e imediato na flexibilidade da empresa, sendo que agora as suas despesas são muito mais inferiores do que anteriormente  <a href="https://aws.amazon.com/solutions/case-studies/ividata"> [20]</a>.</p>  
  
</div>

<br>
<div align="center">
<p>Anterior: <a href="https://github.com/MrBen777/Trabalho_PaaS_Grupo_4/blob/main/Componentes/Servi%C3%A7osAWS.md">Outros Serviços AWS<a> | Próximo: <a href="https://github.com/MrBen777/Trabalho_PaaS_Grupo_4/blob/main/Componentes/Conclus%C3%A3o.md">Conclusão</a></p>
<p><a href="https://github.com/MrBen777/Trabalho_PaaS_Grupo_4/blob/main/README.md">Página Principal</a></p>
<p><a href="https://github.com/MrBen777/Trabalho_PaaS_Grupo_4/blob/main/Componentes/Bibliografia.md">Bibliografia<a></p>
</div>
