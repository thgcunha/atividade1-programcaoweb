# Atividade 1 — Sistema RFID

Projeto simples em HTML e CSS com as duas telas pedidas no roteiro. Para visualizar, abra `ws-cadastro/login.html` no navegador e use o link para a tela de cadastro.

## Requisitos

- `login.html`: usuário ou e-mail, senha, botão **Entrar** e link **Cadastrar-se**.
- `cadastro.html`: nome do produto, código RFID, categoria, preço, botão **Salvar**, um produto de exemplo na lista e uma dica no `aside`.
- Elementos semânticos e rótulos associados aos campos.
- CSS externo compartilhado pelas duas páginas, com media query para telas pequenas.

As páginas representam a interface. Os formulários apontam para `/login` e `/produtos`, mas essas rotas precisam de um backend para autenticar ou salvar dados. A leitura RFID automática também depende de backend; o código pode ser digitado no campo da página.

## Análise e melhorias do site inicial

**Pontos fortes:** as telas já tinham estrutura semântica, campos com rótulos, foco visível e CSS compartilhado. **Pontos fracos:** faltava a configuração de viewport para celular, os títulos das abas eram genéricos e não havia um caminho de volta do cadastro para o login.

As melhorias foram manter os formulários curtos e legíveis, ajustar o título do cabeçalho, adicionar viewport e descrição às páginas, impedir preço negativo e completar a navegação. O CSS usa poucas cores, variáveis e nenhuma biblioteca externa, o que mantém a página leve. Títulos descritivos, descrições e HTML semântico ajudam na identificação das páginas e na acessibilidade.

## Mapa do site

```text
login.html (entrada)
  └── cadastro.html (cadastro de produtos)
        └── login.html (voltar)
```
