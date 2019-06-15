# Typescript

* Что такое Type soundness и Type safety? Есть ли между этими понятиями разница?
* Что такое structural typing, какие есть альтернативы, какие преимущества и недостатки у этого подхода? 
* В каких случаях TS отходит от принципов structural typing и переходит к номинативной типизации для определения compatibility типов?
* Что такое declarations merging, как это работает в TS, какие плюсы и минусы, как объединяются типы для методов?
* Compatibility.
  * Почему TS считает compatible тип функции с меньшим количество аргументов ((a: number) => 0; assignable to (b: number, s: string) => 0;)?
  * И как это распространяется на возвращаемый результат у функций?
  * Можно ли считать из-за этого систему типов TS как unsound?
* Что такое Type Variance?
   *  Где в TS проявляется Covariance, а где Contravariance?
   *  Если в функцию передать коллбек, который принимает другой коллбек, то это будет Covariance или Contravariance (вывести на примере самостоятельно)?
   *  Если бы объекты и классы TS были Invariant, то как бы это повлияло на type safety и на удобство разработки?
* Что такое Type Widening, и какие есть способы его избежать при разработке на TS?
* fresh object literal type:
  * Что это такое?
  * почему для него по-особому включается excess property checking? 
  * Почему передача литерала объекта не напрямую в функцию, а через промежуточное присваивание переменной, делает программу менее типобезопасной?
* Что такое Refinement, и как он работает в контексте Discriminated Unions?
* Почему использование generic переменных в тегах для Discriminated Unions может сделать программу более склонной к багам? Когда это действительно приводит к багам, а когда нет?
* Что такое Companion Object Pattern, и как для его реализации используется Declaration Merging?
* Что такое вывод типов, какие типичные проблемы вывода типов есть, какие типы может выводить TS?
* Какие виды полиморфизма поддерживает TS и как с этим работать?

### Ресурсы
* [What is Type Soundness?](http://jschuster.org/blog/2017/03/21/what-is-type-soundness/)
* [Is there a difference between type safety and type soundness?](https://cs.stackexchange.com/questions/82155/is-there-a-difference-between-type-safety-and-type-soundness)
* [How can a statically typed language support duck typing?](https://softwareengineering.stackexchange.com/questions/252984/how-can-a-statically-typed-language-support-duck-typing)
* [Programming TypeScript by Boris Cherny. Chapter 6.](https://learning.oreilly.com/library/view/programming-typescript/9781492037644/ch06.html)
* [What are covariance and contravariance?](https://www.stephanboyer.com/post/132/what-are-covariance-and-contravariance)
* [What the heck is polymorphism? (только главы до Row polymorphism  включительно)](https://dev.to/jvanbruegge/what-the-heck-is-polymorphism-nmh)
* [Discussion: Typed, modular macros for OCaml, thread about row polymorphism](https://news.ycombinator.com/item?id=13046210)