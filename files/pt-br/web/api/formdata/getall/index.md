---
title: FormData.getAll()
slug: Web/API/FormData/getAll
translation_of: Web/API/FormData/getAll
---
{{APIRef("XMLHttpRequest")}}

O metodo **`getAll()`** do {{domxref("FormData")}} retorna todos os valores associados com a chave dentro `de um objeto FormData`.

> **Nota:** Este metodo esta disponivel no [Web Workers](/pt-BR/docs/Web/API/Web_Workers_API).

## Syntax

```js
formData.getAll(name);
```

### Parametros

- `nome`
  - : O {{domxref("USVString")}} representa o nome da chave que você quer pegar.

### Retorno

Um array de {{domxref("FormDataEntryValue")}}s.

## Exemplo

A seguinte linha cria um objeto `FormData` vazio:

```js
var formData = new FormData();
```

Se nos adicionarmos dois valores oara `username` {{domxref("FormData.append")}}:

```js
formData.append('username', 'Chris');
formData.append('username', 'Bob');
```

A seguinte função `getAll()` retornara um arrat com os valore dentro de `username`:

```js
formData.getAll('username'); // Returns ["Chris", "Bob"]
```

## Especificação

| Specification                                                                        | Status                               | Comment |
| ------------------------------------------------------------------------------------ | ------------------------------------ | ------- |
| {{SpecName('XMLHttpRequest','#dom-formdata-getall','getAll()')}} | {{Spec2('XMLHttpRequest')}} |         |

## Compatibilidade com navegadores

{{Compat("api.FormData.getAll")}}

## Veja também

- {{domxref("XMLHTTPRequest")}}
- [Using XMLHttpRequest](/pt-BR/docs/DOM/XMLHttpRequest/Using_XMLHttpRequest "Using XMLHttpRequest")
- [Using FormData objects](/pt-BR/docs/DOM/XMLHttpRequest/FormData/Using_FormData_Objects "DOM/XMLHttpRequest/FormData/Using_FormData_objects")
- {{HTMLElement("Form")}}
