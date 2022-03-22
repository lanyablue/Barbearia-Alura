##

Imagine que nessas três caixas tendo a primeira sendo o identificador, a segunda sendo a classe, e por último a tag. A tag tem como se fosse uma força 1, a classe uma força 10, e o identificador uma força 100. Toda vez que se utiliza um seletor do tipo “p”, isso quer dizer que a força desse seletor é 1. Quando temos o “form p” a força disso é 1+1, a força disso é 2. Então 2, como é mais forte que o 1, o estilo aplicado vai ser o segundo, do “form p”.

Caso a classe “teste” aplicada naquele “p” com a cor, por exemplo, amarela? A cor do texto ficará amarelo, pois a classe tem uma força 10, ela é superior aos outros dois marcadores inseridos. Então “.teste 10”.
E com um marcador com as seguintes opções: “p.teste {“? Ou seja, só os parágrafos que têm aquela classe terão essa cor, no caso a cor laranja. Somando, a classe tem a força 10, e a tag tem a força 1, então com 11 ele será mais forte que o teste especificamente. E recarregando a página, o texto ficará em laranja.

Por último, o mais forte deles é o identificador. Então o identificador aqui colocando a cor rosa, logo a cor do texto será ser rosa, pois o identificador tem  força 100. Então sempre que  criando CSS, é preciso pensar em o quão específico é o marcador e o quão forte ele vai ser para que não seja sobrescrito por qualquer outro, para que não cometa nenhum erro no código.

##

```
p {       /** valor 1**/
	color: red;
}

form p {  /** valor p 1 + 1 = 2 **/
	color: blue;
}

.teste {   /** valor 10 **/
	color: yellow;
}

p.teste { /** valor 1 + 10 = 11 **/
	color: orange;
}

#teste { /** valor 100 **/
	color: rgb(226, 48, 152);
}
```


#