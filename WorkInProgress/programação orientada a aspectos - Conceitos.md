[Iniciantes](https://www.devmedia.com.br/artigos/iniciantes)[Artigos](https://www.devmedia.com.br/artigos/)[Cursos](https://www.devmedia.com.br/cursos/)[Casos de Sucesso](https://www.devmedia.com.br/depoimentos/)

Navegue

[CRIAR CONTA GRÁTIS](https://www.devmedia.com.br/join/)





Artigo[Invista em você! Saiba como a DevMedia pode ajudar sua carreira.](https://www.devmedia.com.br/introducao-a-programacao-orientada-a-aspectos-conceitos/3062#modulo-mvp)

# Introdução à programação orientada a aspectos - Conceitos

## Este artigo trata sobre AOP - Aspect Oriented Programming, ou programação orientada a aspectos. O objetivo é apresentar primeiramente os conceitos e nas futuras partes do artigo as ferramentas e técnicas.

[Artigos](https://www.devmedia.com.br/artigos/)[Java](https://www.devmedia.com.br/artigos/java)Introdução à programação orientada a aspectos - Conceitos

**Introdução à programação orientada a aspectos - Conceitos**

 

Este artigo trata sobre AOP - Aspect Oriented Programming, ou programação orientada a aspectos. O objetivo é apresentar primeiramente os conceitos e nas futuras partes do artigo as ferramentas e técnicas.

 

Para se fazer um sistema, visando resolver um problema, uma abordagem comum é dividir em partes menores e tratar cada parte separadamente. Esta técnica chama-se separação de interesses.

 

Ao projetar um sistema, trabalhamos com diversos interesses (ou concerns). Na programação orientada a objetos o modelo de abstração trabalha com classes como unidades. No projeto procura-se separar cada interesse em uma classe distinta, porém nem sempre isso é possível.

 

Quando os interesses aparecem misturados numa mesma classe chama-se entrelaçamento, e quando um único interesse aparece espalhado em diversas classes chama-se espalhamento.

 

Para aqueles interesses que não podem ser modularizados em classes dá-se o nome de interesses transversais.

 

Exemplos típicos de interesses transversais são:

·     persistência de objetos

·     segurança de acesso

·     acesso concorrente

·     gerenciamento de transações

·     e muitos outros.

 

A programação orientada a aspectos foi criada para resolver a implementação destes interesses transversais para os sistemas modelados com orientação a objetos. Usando AOP é possível separar estes interesses em unidades chamadas aspectos.

 

Ao desenvolver com AOP a lógica de controle é invertida (Inversion of Control - IoC), pois os aspectos é que conhecem os componentes do sistema, e os componentes desconhecem os Aspectos.

 

Para compor o sistema é preciso fazer o processo de montagem, que consiste em aplicar os aspectos sobre os componentes. Este processo é chamado combinação (weaving) sendo realizado por um combinador (weaver).

 

O weaver pode ser estático, aplicado em tempo de build do sistema, ou dinâmico, aplicado durante a execução do código.

 

O AspectJ é um conjunto de compilador, combinador e utilitários associados a AOP com Java. A sintaxe utilizada no AspectJ para a construção dos aspectos é semelhante a Java, um dos motivos de sua ampla aceitação. Outra vantagem é a utilização do AspectJ sobre a Java Virtual Machine da especificação padrão [JVM], facilitando a migração de código Java para AspectJ.

 

Os principais conceitos na programação de aspectos são:

·     joinpoints - representam eventos de interesse do fluxo de execução. Quando a execução passa por um joinpoint o aspecto pode agir naquele ponto. Exemplo de joinpoints: invocação de métodos, alteração de atributos e exceções.

·     pointcuts - usados para representar um conjunto de joinpoints, pois podem acontecer muitas ocorrências de joinpoints de um mesmo tipo. O AspectJ [ASPECTJ] utiliza expressões regulares na definição de pointcuts.

·     advices - são os procedimentos realizados quando os pointcuts são ativados. Os advices podem ser executados antes (before), depois (after) ou em substituição ao joinpoint. Advices são a implementação dos interesses transversais.

 

Talvez o leitor entenda melhor estes conceitos se pensar que aspectos são estruturas semelhantes a classes, advices são semelhantes a métodos, joinpoints seriam atributos e os pointcuts algo como triggers (gatilhos) sobre os joinpoints.

 

Para utilizar AOP em sistemas reais, de médio e grande porte, é muito importante utilizar uma ferramenta de desenvolvimento. A complexidade de debugar, aplicar e documentar aspectos está no não-determinismo da ordem em que mais de um aspecto sobre o mesmo jointput serão executados.

 

A ferramenta que será usada para demonstrar as técnicas de AOP é o AJDT [AJDT] do projeto Eclipse. Sua distribuição é no formato de um plug-in para o IDE Eclipse, trabalhando integrado ao mesmo.

 

Nas próximas partes deste artigo será visto como instalar o AJDT no Eclipse e algumas aplicações.

 

**Referências**

[JVM] "Java Virtual Machine Specification" - http://java.sun.com/docs/books/vmspec/2nd-edition/html/VMSpecTOC.doc.html

[ASPECTJ] "AspectJ" - http://eclipse.org/aspectj

[AJDT] "AspectJ Development Tools" - http://eclipse.org/ajdt

Tecnologias:

- Orientação a aspectos