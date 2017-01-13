# What's this ?

A palavra chave this no JavaScript confunde desde de jovens à experientes desenvolvedores JavaScript

Usamos this de uma maneira similar como é usado o pronome no Ingles e o  Francês.
Por exemplo, podemos escrever a frase "Clark is a good jornalist because he likes Louis ".
Perceba que usamos "he" ao invés de reescrever Clark, nós podemos ate escrever "Clark is a good jornalist because Clark likes Louis",
 porém, nossos amigos, familia e colegas podem nos abandonar. De forma similar usamos o this como um atalho,
uma referência; que referencia um objeto, que é o sujeito que esta executando o codigo.

Veja esse exemplo:
```js
let pessoa = {
    nome:'Manoel',
    sobrenome:'Freitas'
    nome_completo: function(){
        //Perceba que usamos o this para referenciar este nome e este sobrenome, usamos como se fosse um 
        "he"
        console.log(`${this.nome} ${this.sobrenome}`);

        //Podiamos usar desta forma
        console.log(`${person.nome} ${person.sobrenome}`);
        return this.nome+" "+this.sobrenome;
    }
}
```

Se usarmos person, estaremos acoplando o objeto a variavel, e se digamos o nome da variavel mudar, teriamos que sair mudando o objeto. Além de ficar um pouco ambiguo.
Imagine agora que exista outra variavel global chamada pesssoa que também referenciasse uma propriedade chamada nome, estariamos  acessado a variavel gloval e nao a nossa,
e isto poderia gerar alguns bugs. Então usamos a palavrra "this" não somente por estetica, mas também para precisão. Fazendo o codigo muito menos ambiguo,
 assim como os pronomes nas linguagens naturais.

Assim como "he" é usado para referenciar seu antecessor(substantivo que o pronome se refere), this é similarmente usada para referenciar um objeto cujo uma função e propriedades cque estão ligadas ao objeto.


