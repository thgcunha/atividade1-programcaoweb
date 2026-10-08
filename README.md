# Atividade 1 — Sistema RFID

Projeto simples em HTML e CSS com as duas telas pedidas no roteiro e duas páginas de conta adicionadas depois. Para visualizar, abra `ws-cadastro/login.html` no navegador.

## Requisitos

- `login.html`: usuário ou e-mail, senha, botão **Entrar**, link **Cadastrar-se** e link **Esqueceu a senha?**.
- `cadastro-usuario.html`: nome, e-mail e senha para criar uma conta.
- `recuperar-senha.html`: e-mail para solicitar recuperação de senha.
- `cadastro.html`: nome do produto, código RFID, categoria, preço, botão **Salvar**, um produto de exemplo na lista e uma dica no `aside`.
- Elementos semânticos e rótulos associados aos campos.
- CSS externo compartilhado pelas quatro páginas, com media query para telas pequenas.

As páginas representam a interface. Os formulários apontam para `/login`, `/usuarios`, `/recuperar-senha` e `/produtos`, mas essas rotas precisam de um backend para autenticar, cadastrar, recuperar a senha ou salvar dados. A leitura RFID automática também depende de backend; o código pode ser digitado no campo da página.

## Análise e melhorias do site inicial

**Pontos fortes:** as telas já tinham estrutura semântica, campos com rótulos, foco visível e CSS compartilhado. **Pontos fracos:** faltava a configuração de viewport para celular, os títulos das abas eram genéricos e não havia um caminho de volta do cadastro de produtos para o login.

As melhorias foram manter os formulários curtos e legíveis, ajustar o título do cabeçalho, adicionar viewport e descrição às páginas, impedir preço negativo e completar a navegação. O CSS usa poucas cores, variáveis e nenhuma biblioteca externa, o que mantém a página leve. Títulos descritivos, descrições e HTML semântico ajudam na identificação das páginas e na acessibilidade.

## Mapa do site

```text
login.html (entrada)
  ├── cadastro-usuario.html (criar conta) ── login.html
  ├── recuperar-senha.html (recuperar acesso) ── login.html
  └── cadastro.html (cadastro de produtos) ── login.html
```
