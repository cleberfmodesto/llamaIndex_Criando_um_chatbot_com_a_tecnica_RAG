# llamaIndex_Criando_um_chatbot_com_a_tecnica_RAG

<a href="https://colab.research.google.com/github/cleberfmodesto/llamaIndex_Criando_um_chatbot_com_a_tecnica_RAG/blob/main/Projeto_Final.ipynb" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Abrir_no-Colab-F9AB00?labelColor=F9AB00&logo=googlecolab&logoColor=white" alt="Abrir no Colab"/></a>
<a href="https://github.com/cleberfmodesto/llamaIndex_Criando_um_chatbot_com_a_tecnica_RAG/blob/main/Projeto_Final.ipynb" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Abrir_no-GitHub-0969DA?labelColor=0969DA&logo=github&logoColor=white" alt="Abrir no GitHub"/></a>
<a href="https://codespaces.new/cleberfmodesto/llamaIndex_Criando_um_chatbot_com_a_tecnica_RAG?ref=main" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Abrir_no-Codespaces-1F883D?labelColor=1F883D&logo=github&logoColor=white" alt="Abrir no Codespaces"/></a>

Vamos dar início ao nosso projeto. Atuaremos para a loja Serenatto, que anteriormente era um bistrô e café físico. Eles decidiram expandir os negócios e criar uma página para vender cafés especiais torrados.

Ao verificar a página deles, notaremos que eles vendem alguns grãos especiais, como Bourbon Vermelho, Bourbon Amarelo, um blend especial, Catuaí Amarelo, Geisha e YirgaCheffe.

Identificando o problema da clientela
O problema que a loja enfrenta é que a clientela têm relatado dificuldade para escolher o grão ideal e efetuar a compra. Especialmente quem está começando a conhecer cafés especiais, muitas vezes não sabe como preparar o café e têm dúvidas em geral.

Perguntas como "O que é cada grão?", "Qual é a diferença entre eles?" e "O que é perfil sensorial?" são comuns. Essas dúvidas podem levar a clientela a desistir da compra, pois não consegue decidir o que comprar.

A ideia é implementar um chatbot na página da Serenatto. Assim, a pessoa poderá clicar no chatbot e perguntar sobre os grãos, métodos de preparo e informações sobre a Serenatto. O chatbot fornecerá respostas imediatas, facilitando a interação da clientela e ajudando-a a efetuar a compra.

Utilizando a técnica RAG para gerar respostas precisas
Para criar esse chatbot, utilizaremos uma técnica famosa em inteligência artificial chamada RAG, que significa Retrieval Augmented Generation (Geração Aumentada por Recuperação). Essa técnica possui duas etapas principais:

Recuperação
Geração
Na recuperação, a pessoa abre o chatbot e faz uma pergunta, como "vocês vendem algum café descafeinado?". Precisamos recuperar essa informação de uma base de conhecimento.

Após a recuperação, vem a etapa de geração, onde um modelo de linguagem contextualiza a informação recuperada e responde à pessoa. Um exemplo de resposta é "não temos grão descafeinado, mas temos outras opções."

Criando uma base de conhecimento para o chatbot
A vantagem dessa técnica é que não geramos informações genéricas; fornecemos informações verdadeiras e específicas da Serenatto. Para isso, precisamos criar uma base de conhecimento.

Podemos ter um arquivo contendo as informações que queremos que a pessoa saiba sobre o site. Esse arquivo pode ser em diferentes formatos, como uma planilha ou um arquivo CSV, mas também pode ser um arquivo PDF. Vamos estruturar todas as informações da Serenatto em um arquivo PDF, que servirá como nossa base de conhecimento.

Também é possível combinar arquivos PDF com CSV ou criar uma pasta com diferentes tipos de arquivos, mas focaremos em um arquivo PDF.

Explorando o conteúdo do arquivo PDF
Realizamos vários testes para obter resultados mais interessantes e confiáveis. Esse processo gerou um arquivo PDF que visualizaremos juntos.

.

Esse PDF contém informações da Serenatto, começando com perguntas e respostas gerais. Por exemplo:

P: Quais produtos são vendidos no site da Serenatto?

R: A Serenatto é uma loja online especializada na venda de grãos de cafés especiais, oferecendo grãos torrados, provenientes de fazendas selecionadas de Minas Gerais. Todos os nossos cafés possuem nota SCA acima de 80, garantindo alta qualidade e perfis sensoriais excepcionais.

Outras perguntas incluem a origem dos grãos, quantidade vendida, variedades disponíveis e preços.

Na página seguinte, há mais informações gerais sobre a loja, como prazo de envio, destinos, métodos de pagamento, cursos ou workshops sobre cafés, serviço de assinatura e contatos para dúvidas, como WhatsApp e e-mail.

Estruturando o arquivo por temas
Dividimos o conteúdo por temas. Nas duas primeiras páginas, temos informações gerais. Na terceira página, começamos com informações sobre as variedades dos grãos.

Se alguém quiser mais detalhes sobre o Bourbon Vermelho, por exemplo, encontrará informações sobre doçura, sensação, corpo do café, acidez, etc. Há perguntas sobre todos os tipos de café, variedades, e dúvidas sobre a nota SCA, usada para avaliar a qualidade do café.

Também incluímos informações sobre a produção dos cafés, como a torra e a altitude de cultivo afetam o sabor. Há recomendações de métodos de preparo, como o café coado, com receita e dicas para preparar café gelado, além de outros métodos como espresso e French press. Incluímos dúvidas sobre moagem dos cafés, armazenamento e validade.
