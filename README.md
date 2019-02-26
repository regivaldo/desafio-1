# Desafio CSS
Este conteúdo tem por objetivo auxiliar no aprendizado de CSS e SASS aplicando suas regras em projeto simulado. Serão vários desafios com temáticas específicas, focando em pequenos assuntos para melhor o aprendizado.
Vamos treinar um pouco as técnicas do CSS, focando em uma abordagem dividida em três passos:

* Um protótipo será apresentado
* O HTML estará escrito e não deve ser alterado
* O CSS estará vazio, e ele deve ser escrito para fazer o HTML se comportar corretamente

# Como enviar seu resultado?
* Clone este repositório
* Crie uma branch com seu nome, todo em minusculo: `git checkout -b nome-sobrenome`
* Após finalizado, basta realizar o commit e o push.
* Me envie uma mensagem avisando do seu commit para que eu possa validar seu resultado.

# Desafio 01
Neste desafio, vamos utilizar os sinais do CSS: **>**, **+**, **::**

## Sinal de >
O sinal de > representa um filho direto do elemento anterior.

```css
.classe-pai > .classe-filho-direto
```

Assim, podemos usar para representar uma alteração que só deve afetar um filho direto da classe:

```html
<div class="classe-pai">
  <p>Teste de filho direto</p>
  
  <div class="classe-interna">
    <p>Teste de filho indireto</p>
  </div>
</div>
```

```css
.classe-pai p {  
  color: blue;
}
```
O CSS acima fará com que todos os `<p>` fiquem na cor azul por estar aplicando para todos os filhos de `.classe-pai`.

```css
.classe-pai > p {  
  color: red;
}
```
Já este css, aplicará o tom de vermelho apenas para o `<p>` que está dentro da `.classe-pai` e, não está dentro de outra classe. Assim, o `<p>` que está dentro de `.classe-interna` não receberá a cor vermelha.

# Hora do desafio
Agora, vamos aplicar este conhecimento em alguns HTMLs.
