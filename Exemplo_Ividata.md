Ividata 

A Ividata é uma empresa de consultoria especializada em Big Data, com sede em Paris, fundada no final de 2013. Focando-se na inovação e investindo em investigação e
desenvolvimento, a Ividata criou uma solução de análise de retalho chamada Ivizone que fornece aos comerciantes uma página web acessível por wi-fi, através da qual podem
melhorar os seus esforços de marketing e apresentar ofertas altamente direcionadas aos seus consumidores. Para além do mencionado esta ferramenta também permite fazer o
rastreio de vários dados, tal como; a contagem de visitantes, a duração de cada visita e o tráfico pedonal dentro e nas proximidades das lojas. 

A infraestrutura da Ividata foi inicialmente alimentada por uma série de serviços PaaS providenciados através de diversos fornecedores. Ao utilizar estes serviços a
empresa conseguiu iniciar a produção do Ivizone rapidamente. As vantagens de poder iniciar desenvolvimento dos seus produtos tão rapidamente numa fase tão precoce como
uma empresa eram enormes. 

Rapidamente, a Ividata confrontou-se com despesas crescentes e problemas relativos ao processamento de dados. Estes obstáculos estavam a impor restrições à sua rápida
expansão. De modo a manter o mesmo ritmo de desenvolvimento e evolução, era necessária uma infraestrutura reativa e escalável que permitisse fornecer serviços de
qualidade aos clientes. 

Dados os problemas com as suas infraestruturas anteriores, a decisão de migração baseou-se na escolha de um fornecedor que possibilitasse a melhor relação custo-
eficácia, assim sendo a Ividata optou pela AWS, pois sabia que não iria ter problemas de escalabilidade ou custos. 

Recorrendo aos vários serviços oferecidos pela AWS a implementação passa por adquirir os dados de localização dos smartphones dos clientes, através da rede wi-fi, que
por sua vez é ingerida por um servidor hospedado no AWS Elastic Beanstalk. A Ividata também utiliza Elastic Load Balancing para gerir o tráfego entre instâncias (EC2)
que estão espalhadas por multiplas zonas de disponibilidade. Ou seja, se houver algum problema num datacenter, os sistemas mantêm-se online. 

A posteriori, os registos da análise dos dados são escritos para servidores da Amazon Kinesis, agregados e comprimidos através da Amazon Kinesis Client Library (KCL) e a
AWS Kinesis Connector Library, armazenados no Amazon Simple Storage Service (Amazon S3) e avaliados em tempo real através do Amazon Elastic MapReduce (Amazon EMR), antes
de serem colocados numa base de dados (Amazon RDS). 

A relação custo-eficácia dos serviços de TI é crítica para todas as empresas que trabalham em mercados acelerados. A Ividata desde que migrou para a AWS tem visto um
aumento na agilidade operacional e poupança, relativamente aos custos. 

Os servidores da Ividata, configurados através do AWS Elastic Beanstalk, são cerca de quatro vezes mais rentáveis do que a soluções de PaaS utilizadas anteriormente, o
que teve um impacto importante e imediato na flexibilidade da empresa, sendo que agora as suas despesas são muito mais inferiores do que anteriormente [3].

https://aws.amazon.com/solutions/case-studies/ividata/ [3] 
