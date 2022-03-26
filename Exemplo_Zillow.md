Zillow 

A Zillow, criada por Rich Barton e Lloyd Frink, ex-executivos da Microsoft, é uma empresa americana, fundada em 2004, cujo principal serviço é um marketplace de
imobiliário online [1]. Dezenas de milhões de potenciais compradores e vendedores, assim como agentes e gestores de propriedades, visitam diariamente este marketplace à
procura de casas e apartamentos. A Zillow processa cerca de 3 milhões de novas fotografias diariamente, desde fotos de listagem a imagens de projeto de casa. 

À medida que a empresa aumentou em popularidade e os agentes de imobiliário começaram a fornecer fotografias de maior resolução nas suas listagens, o sistema tradicional
de processamento de imagens da Zillow não conseguiu acompanhar a procura. O sistema era alojado em datacenters On-Premisses e as imagens em si eram fornecidas a uma rede
de entrega de conteúdos (CDN) através de uma queue singular. Este sistema era dispendioso e não era eficiente o suficiente para conseguir lidar com a quantidade massiva
de requests diários 

A Zillow também estava a ter dificuldades com a performance do seu sistema de processamento de imagens. O ritmo a que novas imagens entravam no sistema era
frequentemente elevado, sendo que as possíveis variações na velocidade de acesso às imagens, a partir de certas fontes, causavam a que existisse a possibilidade de que
uma imagem atrasada no topo da queue pudesse impedir que as imagens subsequentes fossem descarregadas. 

A solução para estes problemas baseia-se na escolha de uma arquitetura baseada na cloud que visa resolver os problemas de escalabilidade e desempenho do sistema de
imagens. Optando por usar instâncias da Amazon Elastic Compute Cloud (Amazon EC2) e Amazon Simple Storage Service (Amazon S3) para o armazenamento das imagens, a Zillow
migrou o alojamento e distribuição de imagens de uma instalação On-Premisses para a cloud da AWS.

O AWS Elastic Beanstalk foi utilizado pela Zillow como um meio para criar e fornecer um ambiente de trabalho onde foi desenvolvida uma biblioteca de imagens em Python,
capaz de executar código customizado. Devido às variações na necessidade de capacidade de ingestão de imagens, era necessário um sistema altamente escalável, consoante o
necessário, sendo que o Elastic Beanstalk era a opção mais simples de o conseguir. 

Graças aos serviços da AWS a preocupação com a capacidade dos seus sistemas deixa de ser necessária. A Zillow agora possui a escalabilidade e o desempenho necessário
para exibir aos seus utilizadores imagens de alta qualidade, algo fundamental para a uma experiência de utilizador de qualidade. O download e processamento de imagens
pode ser escalado, de modo a atender a diferentes volumes de imagens recebidas ao longo do dia.[2] 

 

 

https://en.wikipedia.org/wiki/Zillow [1] 

https://aws.amazon.com/solutions/case-studies/zillow/ [2] 
