# Exercise 5 - Dive into Javascript

### Duration
`1 days`

### Code Review
`Trainer + 1`

## Summary
We got information separated into 3 lists - names, roles and hp!

Before you start, download the attached ```.json``` file.

## Guidelines
In this exercise, enter ES6+, an important iteration of ECMAScript (read about it), learn the core changes and new concepts like Arrow Functions, Template Strings, and more to prettify your code, and make it elegant and <b>short</b>

## Tasks
* Assemble a heroes list of objects with the properties mentioned above

  * ```const names = [Mercy, Genji, Zarya]; ```

    ```const roles = [Support, Offense, Tank];```

    ```const getHeroes = ??? ```

    ```console.log(getHeroes()) // - [{name: Mercy, role: Support}, {name: Genji, role: Offense}, {name: Zarya, role: Tank}]```

* Create a groupBy functionality so we can easily classify them by any property. Use role as the default property

  * ```console.log(groupBy(heroes));```
  * ``` { Support: [{name: Mercy, role: Support}], Offense: [{name: Genji, role: Offense}], Tank: [{name: Zarya, role: Tank}]} ```

  * ``` console.log(groupBy(heroes, name)); ```
  * ```{ Mercy: [{name: Mercy, role: Support}], Genji: [{name: Genji, role: Offense}], Zarya: [{name: Zarya, role: Tank}]} ```

* Create a getByRoles that can get what roles we want as parameters

  * ```console.log(getByRoles(heroes, Offense)); // -  [{name: Genji, role: Offense}] ```
  * ```console.log(getByRoles(heroes, Support, Offense)); // -  [{name: Mercy, role: Support}, {name: Genji, role: Offense}] ```

* And last, we want to make all of them nice! Iterate through the heroes and add a functionality to sayHello and print
Hi! My name is ____________, nice to meet you!


  * ```const niceHeroes = makeHeroesNice(getHeroes());```
  * ```niceHeroes[0].sayHello() // - Hi! My name is Mercy, nice to meet you!```