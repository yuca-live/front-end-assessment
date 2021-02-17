# Front-End Assessment

A Yuca oferece um pacote de serviços para que os yukers possam desfrutar da melhor experiência de viver em um Yuca.

Seu desafio é criar um simples aplicação onde o usuário final seria um yuker (morador). Essa aplicação deve permitir que o yuker adicione ou remova serviços contratados no seu pacote de moradia, para desfrutar de mais comodidades ou abrir mão de algumas que ele já não precisa.

## Requisitos

Além dos itens listados abaixo, fique a vontade para adicionar qualquer outra feature que você ache legal, tudo será levado em consideração.

### Requisitos Mínimos
- Criar um aplicação responsiva, de acordo com o layout do Figma
- Ao adicionar e/ou remover serviços o valor final deve ser recalculado corretamente
- Quando o botão 'salvar' for clicado, os serviços selecionados devem ser salvos
- Quando clicar em 'cancelar' as edições feitas devem ser descartadas

### Desejável
- Testes unitários


## Layout

- Layout da aplicação: https://www.figma.com/file/ofetdcZKc2BTuWHkAXJOBv/Teste-Front-End?node-id=0%3A1    
    - (É recomendável logar no Figma para poder ver com mais detalhes os estilos dos componentes)
    - Os links de navegação não precisam ter funcionalidade (só se você quiser colocar alguma coisa para a usabilidade ficar legal)
    - A tela inicial é a página de 'bem vindo'
    - O botão 'contratar serviços' leva a página de serviços

## Mock API Examples

##### /ME [GET] ('https://private-42e99d-yuca1.apiary-mock.com/me')
```
curl 'https://private-42e99d-yuca1.apiary-mock.com/me' \
  -H 'authority: private-42e99d-yuca1.apiary-mock.com' \
  -H 'user-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 11_1_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36' \
  -H 'dnt: 1' \
  -H 'accept: */*' \
  -H 'sec-gpc: 1' \
  -H 'origin: https://jsapi.apiary.io' \
  -H 'sec-fetch-site: cross-site' \
  -H 'sec-fetch-mode: cors' \
  -H 'sec-fetch-dest: empty' \
  -H 'referer: https://jsapi.apiary.io/' \
  -H 'accept-language: en-US,en;q=0.9' \
  --compressed
```

##### /SERVICES [GET] ('https://private-42e99d-yuca1.apiary-mock.com/services')
```
curl 'https://private-42e99d-yuca1.apiary-mock.com/services' \
  -H 'authority: private-42e99d-yuca1.apiary-mock.com' \
  -H 'user-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 11_1_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36' \
  -H 'dnt: 1' \
  -H 'accept: */*' \
  -H 'sec-gpc: 1' \
  -H 'origin: https://jsapi.apiary.io' \
  -H 'sec-fetch-site: cross-site' \
  -H 'sec-fetch-mode: cors' \
  -H 'sec-fetch-dest: empty' \
  -H 'referer: https://jsapi.apiary.io/' \
  -H 'accept-language: en-US,en;q=0.9' \
  --compressed
```

##### /SERVICES [PUT] ('https://private-42e99d-yuca1.apiary-mock.com/services')
```
curl 'https://private-42e99d-yuca1.apiary-mock.com/services' \
  -X 'PUT' \
  -H 'authority: private-42e99d-yuca1.apiary-mock.com' \
  -H 'user-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 11_1_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36' \
  -H 'dnt: 1' \
  -H 'content-type: application/json' \
  -H 'accept: */*' \
  -H 'sec-gpc: 1' \
  -H 'origin: https://jsapi.apiary.io' \
  -H 'sec-fetch-site: cross-site' \
  -H 'sec-fetch-mode: cors' \
  -H 'sec-fetch-dest: empty' \
  -H 'referer: https://jsapi.apiary.io/' \
  -H 'accept-language: en-US,en;q=0.9' \
  --data-binary $'{\n  "userId": 10,\n  "services": [1, 2, 3]\n}' \
  --compressed
```
