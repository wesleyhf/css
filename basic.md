# 1. CSS Básico

CSS (Cascading Style Sheets), assim como o HTML, não é uma linguagem de programação e sim uma linguagem de estilo. Usada para descrever como os elementos são estilizados em páginas HTML.

Atualmente o CSS se encontra em sua versão 3 (CSS3), mas suas novas especificações já estão sendo implementadas (CSS4) e todos esses padrões são definidos e padronizados pela [W3C](https://www.w3.org/Style/CSS/).

# 2. Regras

Basicamente o CSS funciona através de **regras** e utiliza uma série de palavras em inglês para especificar suas propriedades e valores.

Uma regra é constituída em:

- Seletores
- Propriedades
- Valores

## 2.1 Seletores

Seletores são responsáveis por declarar a quais elementos da página o estilo se aplicará, conseguindo assim selecionar um elemento específico ou até mesmo criar grupos de elementos.

Existe uma lista enorme de como filtrar os elementos, por exemplo, conseguimos utilizar a própria `tag`, `atributos`, `estados` e até fazer combinações para selecionar `irmãos` e `filhos`. Você pode conferir mais sobre seletores neste [link](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors).

### Exemplo

```css
p { ... } /* todas as tags p */

p#artigo { ... } /* tags p com o ID 'artigo' */

p.texto { ... } /* tags p com a classe 'texto' */

p > * { ... } /* filhos da tag p */

p * { ... } /* todas as tag dentro da p */

/* não se esqueça que podemos misturar todas elas */
p#artigo > p.texto * { ... } /* dezenas de possibilidades */
```

## 2.2 Propriedades

Propriedades são os responsáveis por alterar os atributos visuais dos elementos filtrados pelos **Seletores**. Você pode conferir mais propriedades neste [link](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#Keyword_index).

### Exemplos

```css
p { /* todas as tags p */
  color: ...; /* terá sua cor alterada */
}

p#artigo { /* tags p com o ID 'artigo' */
  background: ...; /* terá seu fundo alterado */
}
```

## 2.3 Valores

Valores são os estilos exato que você deseja aplicar para um atributo, podendo ser eles `cores`, `unidades` e valores específicos de cada atributo.

### Exemplo

```css
p { /* todas as tags p */
  color: red; /* terá sua cor de texto vermelha */
}

p#artigo { /* tags p com o ID 'artigo' */
  background: blue; /* terá seu fundo azul */
  width: 1000px; /* e largura de 1000 pixels */
}
```

No exemplo acima utilizamos `px` (pixels), que é um valor de unidade. Você pode conferir mais sobre unidades neste [link](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Values_and_units)
