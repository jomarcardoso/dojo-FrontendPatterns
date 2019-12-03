# dojo-JavaScriptPatterns
Padrões e boas práticas que acho útil compartilhar.

## Padrões

Padrões são criados para suprir uma necessidade da linguagem, organização, entendimento, segurança entre outros.

### Módulos

Protege as variáveis e facilita na nomenclatura das variáveis em um escopo menor.

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

O `restArgs` serve para pegar todos os outros atributos que não serão usado e colocar em um objeto. Bastante utilizado nos componentes em React para enviar os "props" para o primeiro elemento que ele renderiza.

## Boas práticas

### Tipos de arquivos

- views
- services
- costants
