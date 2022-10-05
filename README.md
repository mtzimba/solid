# S.O.L.I.D

_SOLID_ é um acrônimo dos 5 princípios de _design_ da programação orientada a objetos (POO). Estes princípios foram apresentados por [Robert C. Martin _(Uncle Bob)_](https://en.wikipedia.org/wiki/Robert_C._Martin) no ano de 2000 através de seu artigo [_Principles Of Ood_](http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod). Estes princípios são:

<html>
<body>
<!--StartFragment-->

Sigla | Princípio
--|--
**S**RP | _Single Responsibility Principle_ - Responsabilidade única
**O**CP | _Open Closed Principle_ - Aberto/Fechado
**L**SP | _Liskov Substitution Principle_ - Substituição de Liskov
**I**SP | _Interface Segregation Principle_ - Segregação de interface
**D**IP | _Dependency Inversion Principle_ - Inversão de dependência

<!--EndFragment-->
</body>
</html>

O uso destes princípios no projeto de _design_ de classes da POO ajuda a manter um código melhor estruturado, diminuindo o acoplamento entre classes, com isso, ganhando em legibilidade, testabilidade e manutenibilidade do mesmo.

## **S** - _Single Responsibility Principle_ - Responsabilidade única

Robert C. Martin define este princípio como: _Uma classe deveria ter uma e apenas uma razão para mudar_. Neste contexto, quando observa-se uma classe com muitas atribuições é um sinal que este princípio foi quebrado. Isso remete a imagem do canivete suíço com várias atribuições num mesmo lugar, conforme imagem abaixo.

![canivete_suico](https://user-images.githubusercontent.com/2261749/191259000-cf605f34-5f99-4e74-8f7e-95e571d4d62d.png)

Desta forma, toda vez que for realizada alguma manutenção em uma destas atribuições (funcionalidades), faz com que aumente a chance impacto em outros pontos. Classes que são construídas neste formato devem ser quebradas em classes mais especialista para cada atribuição especifica. Isso facilita a manutenção do código, pois a alteração é num ponto especifico, na criação de testes e na diminuição da concorrência nas alterações num mesmo lugar.

## **O**CP - _Open Closed Principle_ - Aberto/Fechado

## **L**SP - _Liskov Substitution Principle_ - Substituição de Liskov

## **I**SP - _Interface Segregation Principle_ - Segregação de interface

## **D**IP - _Dependency Inversion Principle_ - Inversão de dependência

Robert C. Martin define este princípio como: _Dependa de abstrações e não de implementações_. Este princípio está ligado diretamente ao acomplamento de classes. Orienta o uso de abstrações (intefaces e classes abstratas) pois estas tendem a mudar menos, são mais estáveis. Desta forma, por sofretem poucas alterações, dificilmente vão introduzir problemas nas classes principais que fazem uso delas.

Um exemplo bem claro do uso deste principio são as abstrações que são usadas para conexões com banco de dados. Elas ajudam a quebrar o acoplamento forte das implementações de um banco de dados específios, como por exemplo MySQL.

## Referências 

1. http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod
2. https://www.freecodecamp.org/portuguese/news/os-principios-solid-da-programacao-orientada-a-objetos-explicados-em-bom-portugues/
3. https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design-pt
4. https://www.youtube.com/watch?v=rnWPWU7XKeg
5. https://www.baeldung.com/solid-principles
6. https://www.casadocodigo.com.br/products/livro-oo-solid
