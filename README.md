# Introdução à Ciência da Computação (UNIVALI), com Felipe Viel: aplicação em Python - Caio César Sabino Soares e Isis Tristão
###### Repositório criado com a finalidade de demonstrar uma aplicaçao em Python para uma atividade da disciplina de Introdução à Ciência da Computação, da UNIVALI.


## Introdução: o que é Python e para que serve?
Criada pelo holandês **Guido Van Rossum** com sua primeira versão no ano de **1990**, Python é uma linguagem **Open-Source** de propósito geral usado bastante em **data science**, **machine learning**, **desenvolvimento de web**, **desenvolvimento de aplicativos**, **automação de scripts*, **fintechs** e mais. Descendente da linguagem de programação *ABC* e tendeu seu nome baseado na série de comédia *The Monty Python's Flying Circus*, a linguagem é fácil de aprender, altamente legível (~~afirmação passível de questionamentos~~) e fácil de usar.

> O **[StackOverflow](https://pt.stackoverflow.com/questions/tagged/python)** considerou Python a linguagem de renome que **mais cresce**, e a linguagem que os programadores mais > desejam aprender. Como por exemplo em 2014 nos Estados Unidos, 80% das 10 melhores universidades de ciência da computação (e 69% dos top 39) ensinam o python em cursos 
> introdutórios.
> Algumas características da linguagem:
> 
> * Fácil de ler, escrever e der ser mantido, então os desenvolvedores ❤️ isso
> * Eficiente para fazer protótipos, então Startups e empreendedores ❤️ isso 
> * Altamente escalável e poderoso, grandes empresas como Google e Netflix ❤️ isso 
> * Moldável: você consegue facilmente acessar e adicionar bibliotecas para funções específicas, então cientistas de dados & engenheiros de Machine Learning ❤️ isso.
> * Uma linguagem de programação Open-Source com uma grande comunidade, portanto todo mundo ❤️ isso.
> 
> Fonte: [Harve - Python para que serve: top 5 utilidades](https://harve.com.br/blog/programacao-python-blog/python-para-que-serve-top-5-utilidades/)


## Sobre a aplicação escolhida: **Processamento de imagens - Detecção bordas com o OpenCV e algoritmo Canny**

Após algumas pesquisas, a dupla, em consenso, escolheu a temática de **processamento de imagens**, tendo em vista a sua utilidade e ampla utilização na contemporaneidade. Durante a explicação do professor e a menção do Canny como mecanismo de detecção de bordas em imagens digitais, surgiu em nós a vontade de realizar alguns teste para ver a mágica funcionando. Tivemos alguns pequenos interpéreos na hora de realizar a aplicação do código que, deixando claro, **não é de nossa autoria** e sim de um website chamado **Caderno de Laboratório**, onde o passo a passo para realizar a detecção de bordas está descrito. Fizemos uma leitura atenciosa dos procedimentos para compreensão do algortimo e posteriormente, com a ajuda dos documentos disponibilizados pelo professor via **[Google Colab](https://colab.research.google.com/drive/18giPTkiHBGlt0DY1lOjPRA7qP0OGh37o?usp=sharing)**, conseguimos implementar com sucesso o algoritmo dentro desta última plataforma supracitada.

Com base nos resultados, observamos que, após o processamento, a imagem não tinha todas as bordas definidas perfeitamente, mas era evidente o reconhecimento quando comparada com a imagem original. Há uma boa distância entre os pixels de borda que é detectada e os pixels da borda real. Ademais, os valores no meio dos limiares são analisados em conjunto com os vizinhos. Se o vizinho é uma borda, eles são considerados borda. Se não, são descartados. Isto, eventualmente, pode causar uma incoerência facilemtne perceptível quando analisamos o resultado. 

Mas, de modo geral, achamos a aplicação escolhida incrível. Fizemos testes com imagens reais do nosso dia a dia, tornando a experiência ainda mais intrigante. A aplicação é amplamente utilizada por **carros autônomos**, por exemplo. Além disso, é evidente que os seres humanos, como espécie altamente desenvolvida, tem a habilidade de distinguir objetos em um ambiente com certa facilitade, tendo em vista sua visão avançada em conjunto com suas capacidades cerebrais. No entanto, a máquina não age da mesma forma. Ela não tem "olhos", como nós, mas tem câmeras. Estes dispositivos de visualização aplicados à detecção de bordas (como esta), conseguem aos poucos perceber e distinguir objetos em mesas, caixas, cenários, cidades e afins. Isso pode ser útil quando se utiliza câmeras aplicada à **robótica**, **eletrodomésticos de limpeza**, **máquinas industriais de seleção e organização** e por aí vai.

> A capacidade de detectar bordas em uma imagem é muito interessante em diversas situações. Existem muitas formas diferentes de se detectar bordas com o opencv. Hoje veremos uma 
> função implementada no OpenCV que já processa todos os passos intermediários necessários para a detecção de bordas.
> Referência para a aplicação: [Carderno de Laboratório - Detectar bordas com o OpenCV](https://cadernodelaboratorio.com.br/detectar-bordas-com-o-opencv-4-2/)
