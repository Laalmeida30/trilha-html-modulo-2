# Clínica Veterinária São Francisco

> Projeto educativo — site estático (HTML/CSS) da Trilha HTML - Módulo 2.

Abra `trilha-html-modulo-2/paginaprincipal.html` no VS Code e use a extensão Live Server para visualizar a página localmente.

Extensões úteis: `Live Server`, `Prettier`, `ESLint`, `GitLens`, `Path Intellisense`.

Para formatação automática, a configuração do workspace já define Prettier como formatador e `formatOnSave`.

## Como visualizar

1. Instale a extensão Live Server no VS Code.
2. Abra `trilha-html-modulo-2/paginaprincipal.html` e clique em "Go Live" (Live Server).

## Notas rápidas

- Validação simples do formulário de contato foi adicionada em `contato/index.html`.
- O `base.css` recebeu ajustes de responsividade para telas menores (<= 900px).
 
## Melhorias adicionadas

- Meta tags (`description`, `canonical`) e Open Graph em todas as páginas.
- Link "Pular para o conteúdo" (`.skip-link`) e roles ARIA (`role="navigation"`, `role="main"`).
- `srcset` e `sizes` nas imagens de cabeçalho para carregamento responsivo.
- Content Security Policy (meta) básica adicionada nas páginas.
- Servidor stub em `/server` para receber `POST /contact` (exemplo com Express).
- Workflow GitHub Actions em `.github/workflows/ci.yml` verificando Prettier e HTMLHint.

## Rodando o servidor stub

```bash
cd server
npm install
npm start
```

O servidor rodará em `http://localhost:3000` e aceitará `POST /contact`.
# Trilha HTML - Dio.me
## Módulo 02 - HTML I - Conceitos Básicos

Este desafio tem como objetivo, criar um site "quase" completo, com tudo o que vimos neste módulo. Os temas que deverão ser abordados são:
- Formulários
- Estruturação e formatação de texto
- Mídias
- Tabelas

Além de outros recursos falados nas aulas!

## Instruções
1. Você deve criar um site de uma clínica médica (você escolhe a especialidade)
2. Este site deve conter o seguinte menu de navegação:
    - Página Principal
    - Sobre a clínica
    - Horário de Atendimento
    - Contato
3. Deve, obrigatoriamente, utilizar todas os assuntos abordados nas aulas.

Abaixo como cada página deve ser criada e estruturada.

### Estrutura das páginas

Todas as páginas terão que seguir um padrão pré-definido. Como não aprendemos sobre CSS ainda, utilize o arquivo `template.html` para utilizar como base. Ele segue uma estrutura semelhante a image abaixo.

![Estrutura](https://i.stack.imgur.com/9jI6f.gif)

\* _No template tem algumas cores mas é apenas para melhor visualização. Fique a vontade para alterar da melhor forma._

No **Menu**, ficará localizado o menu de navegação (ah vá!), no **Header** de cada página ficará uma imagem, no **Footer** informações de contato, e o **Content** é o conteúdo de cada página.
### Página Principal
1. Deve ter uma imagem no **Header**.
2. Em **Content** uma breve descrição sobre a clínica.
3. **Menu** e **Footer** padrões em todas as páginas.

### Sobre a clínica
1. Deve ter uma imagem diferente no **Header**.
2. Em **Content** um texto falando sobre a clínica.
3. **Menu** e **Footer** padrões em todas as páginas.

### Horário de Atendimento
1. Deve ter uma imagem diferente no **Header**.
2. Em **Content** um pequeno texto falando sobre os serviços, e uma tabela de preços, onde cada linha é um serviço, com o preço de cada um de acordo com os dias da semana.

|Serviços |Segunda a Sexta | Sábados | Feriados |
|---|---|---|---|
|Clínica geral | 08h - 19h  | 08h - 14h | 08h - 14h  |
|Psicologia | 08h - 19h  | 08h - 14h | 08h - 14h  |
|Pediatria | 08h - 19h  | 08h - 18h | - |
|Oftalmologia | 08h - 19h  | 08h - 18h | - |
|||||

3. **Menu** e **Footer** padrões em todas as páginas.


### Contato
1. Deve ter uma imagem diferente no **Header**.
2. Em **Content** deve ter:
    - Os telefones de contato (celular e whatsapp)
    - Endereço completo da clínica
    - Um Iframe com o Google Maps apontando o endereço da clínica
    - Um formulário de contato com:
        - Nome (type="text")
        - E-mail (type="email")
        - Assunto (type="text")
        - Mensagem (textarea)
        - Botões de envias e limpar formulário

3. **Menu** e **Footer** padrões em todas as páginas.

Desafio está lançado! Com tudo que aprendemos no Módulo II é perfeitamente possível criar este site! 

Bora pra cima!