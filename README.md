# Dev Typist Pro

> Um jogo educacional de digitação e programação que combina progressão
> idle/clicker, prática de sintaxe e desafios rápidos de lógica.

## Sobre o projeto

**Dev Typist Pro** é um projeto web educacional pensado para transformar
o estudo de programação em uma experiência curta, progressiva e
divertida. A proposta é permitir que o usuário entre para passar alguns
minutos jogando e, durante esse processo, pratique digitação de código,
reconheça sintaxes, resolva desafios e acompanhe sua evolução.

O projeto funciona diretamente no navegador e foi desenvolvido como uma
aplicação front-end em um único `index.html`, com autenticação e
sincronização de progresso pelo Supabase.

## Principais recursos

-   Terminal de digitação de código com feedback em tempo real.
-   Suporte a HTML/CSS, Python, Java, PHP, SQL e TypeScript.
-   Sistema de LOC (Lines of Code) como recurso principal do jogo.
-   Combo de digitação, WPM/CPM e estatísticas de desempenho.
-   Loja de upgrades dividida em Equipe, Skills e Hardware/Software.
-   Conquistas e metas de progressão.
-   Eventos de servidor e deploy de emergência.
-   Temas visuais e interface multilíngue.
-   Efeitos sonoros e batida eletrônica minimalista de fundo.
-   Autenticação por e-mail/senha e Google.
-   Modo visitante.
-   Salvamento local e sincronização de progresso em nuvem.
-   Tutorial de introdução:
    -   visitante recebe o tutorial em novas entradas;
    -   contas autenticadas concluem ou pulam o tutorial apenas uma vez.
-   Sistema educacional com XP e níveis.
-   Progressão de carreira: Iniciante, Estagiário, Dev Júnior, Dev
    Pleno, Dev Sênior e Tech Lead.
-   Combo Dev para recompensar desafios respondidos sem dica.
-   Microlições de programação.
-   Desafios rápidos de interpretação de código.
-   Caça-bugs.
-   Missões diárias e sequência de estudo.
-   Domínio individual por linguagem.
-   Projetos de carreira com objetivos progressivos.

## Objetivo educacional

O jogo trabalha com três etapas complementares:

**Digitar → Entender → Resolver**

A digitação cria familiaridade com código e sintaxe. As microlições
apresentam conceitos em pequenas doses. Os desafios e caça-bugs exigem
interpretação e raciocínio.

O objetivo não é substituir cursos, documentação ou prática de
desenvolvimento real, mas funcionar como uma ferramenta complementar de
estudo e contato frequente com programação.

## Tecnologias

  Tecnologia           Uso
  -------------------- --------------------------------------
  HTML5                Estrutura da aplicação
  CSS / Tailwind CSS   Interface e responsividade
  JavaScript           Lógica do jogo
  Supabase             Autenticação e persistência em nuvem
  Font Awesome         Ícones
  Web Audio API        Sons e batida de fundo
  LocalStorage         Progresso local e modo visitante
  Vercel               Hospedagem/deploy web

## Estrutura atual

``` text
/
├── index.html
└── README.md
```

A versão atual concentra interface, estilos e lógica no `index.html`.
Isso facilita testes e deploys rápidos. Em uma evolução futura, o
projeto pode ser dividido em módulos (`css/`, `js/`, `assets/`) sem
alterar a experiência do usuário.

## Como executar localmente

Clone o repositório:

``` bash
git clone https://github.com/script33dt-glitch/Dev-game-.git
cd Dev-game-
```

Depois, abra o projeto com um servidor local. No VS Code, uma opção
simples é usar uma extensão de servidor local e abrir o `index.html`.

Também é possível usar:

``` bash
python -m http.server 5500
```

Depois acesse `localhost:5500` no navegador.

> Para testar corretamente autenticação OAuth, utilize uma origem/URL
> autorizada na configuração do Supabase.

## Supabase

O projeto utiliza o Supabase para autenticação e sincronização do
progresso das contas.

Fluxos suportados:

-   e-mail e senha;
-   Google OAuth;
-   visitante sem sincronização em nuvem.

O progresso autenticado é associado ao usuário, permitindo que recursos
como conclusão do tutorial e evolução sejam recuperados em novos
acessos.

### Segurança

A chave pública/anon do Supabase pode ser utilizada no cliente, mas
**não deve ser tratada como mecanismo de segurança**. A proteção dos
dados deve ser feita no banco com políticas de **Row Level Security
(RLS)**, garantindo que cada usuário possa ler e alterar somente o
próprio progresso.

Nunca coloque no front-end chaves `service_role`, senhas privadas ou
outros segredos administrativos.

## Deploy

O projeto pode ser publicado como site estático.

### Vercel

1.  Importe o repositório do GitHub na Vercel.
2.  Use o diretório raiz do projeto.
3.  Para a versão atual, não é necessário processo de build.
4.  Faça o deploy.
5.  Adicione o domínio final às URLs permitidas de autenticação/redirect
    no Supabase.

Cada `push` na branch configurada para produção pode gerar um novo
deploy automaticamente.

## Fluxo básico do jogador

``` text
Abrir o jogo
      ↓
Entrar / Criar conta / Visitante
      ↓
Tutorial (quando aplicável)
      ↓
Digitar código
      ↓
Ganhar LOC + XP
      ↓
Comprar upgrades
      ↓
Resolver desafios e bugs
      ↓
Aumentar domínio e carreira
      ↓
Completar missões e projetos
```

## Progressão educacional

O projeto separa a economia do jogo do aprendizado:

-   **LOC:** recurso econômico usado na progressão e upgrades.
-   **XP:** representa progresso educacional/carreira.
-   **Domínio:** acompanha experiência em cada linguagem.
-   **Combo Dev:** recompensa respostas corretas sem utilização de
    dicas.
-   **Missões:** incentivam sessões curtas e recorrentes.
-   **Projetos:** funcionam como objetivos maiores de progressão.

Essa separação evita que apenas deixar o jogo rodando represente
automaticamente domínio de programação.

## Público-alvo

O Dev Typist Pro é pensado principalmente para:

-   pessoas iniciando em programação;
-   estudantes que querem praticar sintaxe;
-   usuários interessados em melhorar familiaridade com código;
-   jogadores casuais que gostam de progressão e idle games;
-   professores que desejam apresentar programação de forma mais leve e
    interativa.

## Roadmap

Algumas possibilidades para versões futuras:

-   ampliar o banco de desafios e microlições;
-   criar trilhas específicas por linguagem;
-   adicionar projetos educacionais mais completos;
-   painel de estatísticas de estudo;
-   sistema de revisão de conteúdos com maior índice de erro;
-   acessibilidade e navegação completa por teclado;
-   versão PWA instalável;
-   testes automatizados;
-   modularização do JavaScript e CSS;
-   painel administrativo para criação de novos desafios;
-   recursos opcionais para professores/turmas.

## Boas práticas para contribuição

Ao adicionar uma funcionalidade:

1.  preserve o funcionamento das mecânicas existentes;
2.  teste modo visitante e conta autenticada;
3.  teste salvamento local e sincronização em nuvem;
4.  verifique a experiência em desktop e celular;
5.  evite armazenar segredos no front-end;
6.  mantenha os desafios educacionais curtos e objetivos;
7.  faça commits com mensagens claras.

Exemplo:

``` text
feat: adiciona desafios de Python
fix: corrige persistência do tutorial
ui: melhora painel de progresso
docs: atualiza README
```

## Status

🚧 **Em desenvolvimento ativo**

O projeto está em fase de testes e evolução. Mecânicas, balanceamento,
conteúdos educacionais e interface podem mudar conforme novos testes
forem realizados.

## Autor

**Arthur Pereira Bolognesi**

Projeto desenvolvido como uma experiência que une programação, estudo,
gamificação e entretenimento.

## Licença

A licença do projeto ainda deve ser definida. Antes de aceitar
contribuições externas ou permitir redistribuição, recomenda-se
adicionar um arquivo `LICENSE` ao repositório.

------------------------------------------------------------------------

**Dev Typist Pro** --- aprender programação também pode parecer um jogo.
