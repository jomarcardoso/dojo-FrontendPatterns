# Frontend Pattterns

Padrões e boas práticas que acho útil compartilhar.

## Padrões

Padrões são criados para suprir uma necessidade da linguagem, organização, entendimento, segurança entre outros.

### Módulos

Protege as variáveis e facilita na nomenclatura das variáveis em um escopo menor.

### VASC

> Views, APIs, Services e constantes

É uma forma de organização dos componentes no frontend.

#### Views

Cuidam da renderização.

#### Services

Funções que auxiliares.

#### API

Conjunto de Funções auxiliares com um propósito e um resultado testável.

#### Constants

Mensagens, caminhos...

### Argumento único

Quando precisar colocar mais do que um argumento colocar em um objeto para eles serem nomeados e poderem ser ignorados se necessário.

```js
function doSomething(arg) {
  // ...
}
```

```js
function doSomething({ arg1, arg2, ...restArgs } = {}) {
  // ...
}
```


```js
function doSomething(props = {}) {
  // props.arg1
  // props.arg2
  // ...
}
```

O `restArgs` serve para pegar todos os outros atributos que não serão usado e colocar em um objeto. Bastante utilizado nos componentes em React para enviar os "props" para o primeiro elemento que ele renderiza.

## Boas práticas

### Tipos de arquivos

- views
- services
- costants
