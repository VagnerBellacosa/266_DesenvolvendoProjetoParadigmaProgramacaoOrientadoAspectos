[Artigos](https://www.treinaweb.com.br/blog)O que é AOP - Programação Orientada a Aspectos?

Atualmente, existem vários [paradigmas de programação](https://www.treinaweb.com.br/blog/linguagens-e-paradigmas-de-programacao/), como por exemplo o [paradigma orientado a objetos](https://www.treinaweb.com.br/blog/os-pilares-da-orientacao-a-objetos/), onde temos instâncias de classes trocando mensagens entre si. Da mesma forma, também temos o paradigma funcional, onde podemos falar que existem funções que seguem alguns conceitos matemáticos interagindo entre si. Hoje, vamos abordar um outro tipo de paradigma: o **AOP - Aspect Oriented Programming**, ou **Programação Orientada a Aspectos**.



[![img](https://dkrn4sk0rn31v.cloudfront.net/uploads/2023/06/ebook-logica-de-programacao.jpg)](https://www.treinaweb.com.br/ebook/logica-de-programacao/)



### O que é a Programação Orientada a Aspectos?

O paradigma orientado a aspectos é um paradigma baseado em **meta informações**. Primeiramente devemos saber que meta informação é, resumidamente, uma “informação de uma informação”.

Por exemplo, vamos imaginar o seguinte: você tem um carro e esse carro é da cor **“preta”**. Essa é uma informação do carro, porém “preta” é um atributo. “Cor” seria uma meta informação do carro em um contexto onde a informação a ser tratada é o veículo em si. Já “preta” seria o valor do atributo “cor”, mas esse valor de atributo só tem “significado” ou “força” se sabermos sobre o que “cor” se trata, ou seja: se soubermos a meta informação – ou significado – de “cor”.

Às vezes, nos deparamos com responsabilidades que são difíceis de isolar ou que exigem a escrita de código que não fazem parte do domínio da aplicação; porém, ainda dizem respeito à aspectos essenciais.

A programação orientada a aspectos vem para nos ajudar nisso, pois é uma abordagem que permite a separação dos componentes funcionais de uma forma concisa, utilizando-se de mecanismos de abstração e de composição. O termo “aspecto” se refere aquilo que faz parte da aparência de algo.

O objetivo da programação orientada a aspectos é oferecer suporte para o desenvolvedor na tarefa de separar componentes entre si e os aspectos entre si, utilizando-se de mecanismos que permitam a abstração e composição destas.

Alguns exemplos seriam o gerenciamento de transações, logs, cache, indexação de dados etc.

### Alguns conceitos…

• **Join points:** são os pontos que possuem algum aspecto associado. São os métodos da aplicação que necessitam da execução de algum aspecto;

• **Point cuts:** são expressões que identificam os join points, onde podemos usar namespaces, classes e expressões regulares para identificar os join points;

• **Advices:** são fragmentos de código que contêm o comportamento de um aspecto. Existem alguns tipos como Before, After e outros, onde cada um define em que momento da execução do join point, o comportamento do aspecto deverá ocorrer.



![Swift - Criação de aplicações móveis para IOS Básico](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/swift.svg)

##### CursoSwift - Criação de aplicações móveis para IOS Básico

[Conhecer o curso](https://www.treinaweb.com.br/curso/desenvolvimento-de-aplicacoes-ios-com-swift-basico)



### Por que utilizar esse paradigma?

Como esse paradigma geralmente envolve conceitos que independem da camada e não tem relação direta com os requisitos funcionais de um sistema, temos alguns benefícios como a reutilização, clareza e desacoplamento do código.

A programação orientada a aspectos também possibilita fazer a devida separação de responsabilidades, considerando funcionalidades que são essenciais para um grupo de objetos, mas não são de responsabilidade direta deles.