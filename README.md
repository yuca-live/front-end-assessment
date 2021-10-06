# Yuca Front-End Assessment

## Descrição

A Yuca oferece um pacote de serviços para que os yukers possam desfrutar da melhor experiência de viver em um Yuca.

Seu desafio é criar uma aplicação que permita que o yuker adicione ou remova serviços contratados no seu pacote de moradia, para desfrutar de mais comodidades ou abrir mão de algumas que ele já não precisa.
<br><br>

## Layout

Acesse o [Figma](https://www.figma.com/file/ofetdcZKc2BTuWHkAXJOBv/Teste-Front-End?node-id=0%3A1)


[![Layout Mobile](./mobile.png "Layout Mobile")](https://www.figma.com/file/ofetdcZKc2BTuWHkAXJOBv/Teste-Front-End?node-id=0%3A1)

*É recomendável logar no Figma para poder ver com mais detalhes os estilos dos componentes*
- A Tela inicial é a "Meu Yuca"  ("Bem-vindo, Bernardo")
- Tela "Serviços" é uma subseção da tela "Meu Yuca"
- Link "Minha Conta" não tem funcionalidade (só se você quiser colocar alguma coisa para a usabilidade ficar legal)
<br><br>

## Critérios de aceite funcionais
- Criar estrutura responsiva
- Criar tela inicial "Meu Yuca"
- Criar tela "Serviços"
  - Ao adicionar e/ou remover serviços o valor exibido deve ser atualizado
  - Quando o botão 'salvar' for clicado, os serviços selecionados devem ser salvos usando a api de mock (\*)
  - Quando clicar em 'cancelar' as edições feitas devem ser descartadas

<br>

*(\*) mock server não persistirá os dados*

<br><br>
## O que será analisado?

A ideia do teste é termos uma noção do seu conhecimento, portanto o quão mais completa e "pronta pra produção" essa aplicação estiver, melhor. Qualquer framework frontend que já use no seu dia-a-dia pode ser usado.

O nível de senioridade da vaga será levado em consideração nesta análise.

### Infraestrutura
- setup de desenvolvimento
- setup de build/deploy/ci etc
- setup de testes

### Aplicação
- escolha e domínio do framework utilizado (react/vue/swelte/angular/vanilajs)
- cobertura de testes
- arquitetura 

### Layout
- acuidade visual
- responsividade
- organização/modularização/componentização dos estilos, o que escolher usar

<br><br>
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
