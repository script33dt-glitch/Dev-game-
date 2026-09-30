::: {align="center"}
# ⌨️ Dev Typist Pro

### `CODE • TYPE • LEARN • LEVEL UP`

**🇧🇷 Transforme estudo de programação em jogo.**\
**🇺🇸 Turn programming practice into a game.**

`HTML/CSS` • `Python` • `Java` • `PHP` • `SQL` • `TypeScript`

------------------------------------------------------------------------

> 🟢 **STATUS: EM DESENVOLVIMENTO / IN DEVELOPMENT**
:::

## 🇧🇷 Português

### 🎮 Sobre o Dev Typist Pro

**Dev Typist Pro** é um jogo educacional web que mistura **digitação de
código, programação, progressão idle/clicker e desafios rápidos de
lógica**.

A ideia é simples: você pode abrir o jogo para passar alguns minutos,
evoluir sua carreira virtual e, ao mesmo tempo, manter contato frequente
com conceitos e sintaxes de programação.

O projeto segue três pilares:

``` text
⌨️ DIGITAR  →  🧠 ENTENDER  →  💡 RESOLVER
```

Digitar ajuda na familiaridade com a sintaxe. Microlições apresentam
conceitos de forma rápida. Desafios e caça-bugs incentivam interpretação
e raciocínio.

> O objetivo não é substituir cursos, documentação ou projetos reais,
> mas funcionar como uma ferramenta complementar e divertida de prática.

### ✨ Recursos

``` text
┌──────────────────────────────────────┐
│            DEV TYPIST PRO            │
├──────────────────────────────────────┤
│  ⌨️ Terminal de código               │
│  📈 LOC + XP + níveis                │
│  🔥 Combo de digitação / Combo Dev   │
│  🧠 Desafios de programação          │
│  🐛 Caça-bugs                        │
│  📚 Microlições                      │
│  🎯 Missões diárias                  │
│  🏆 Conquistas                       │
│  🛒 Upgrades                         │
│  💼 Carreira de desenvolvedor        │
│  ☁️ Progresso em nuvem               │
└──────────────────────────────────────┘
```

O jogo conta atualmente com:

-   terminal de digitação com feedback em tempo real;
-   HTML/CSS, Python, Java, PHP, SQL e TypeScript;
-   LOC (Lines of Code) como recurso econômico;
-   XP e níveis de carreira;
-   progressão de **Iniciante → Estagiário → Dev Júnior → Dev Pleno →
    Dev Sênior → Tech Lead**;
-   WPM/CPM, combo e estatísticas;
-   domínio individual por linguagem;
-   microlições;
-   desafios de interpretação de código;
-   caça-bugs;
-   missões diárias e sequência de estudo;
-   projetos de carreira;
-   loja de Equipe, Skills e Hardware/Software;
-   conquistas;
-   eventos de servidor e deploy de emergência;
-   temas visuais;
-   interface multilíngue;
-   efeitos sonoros e batida eletrônica minimalista;
-   login por e-mail/senha e Google;
-   modo visitante;
-   salvamento local e sincronização pelo Supabase;
-   tutorial inteligente para novos jogadores.

### 🕹️ Loop do jogo

``` text
              ┌──────────────┐
              │ DIGITAR CÓDIGO│
              └──────┬───────┘
                     ↓
              ┌──────────────┐
              │ GANHAR LOC/XP │
              └──────┬───────┘
                     ↓
        ┌────────────┴────────────┐
        ↓                         ↓
 ┌─────────────┐           ┌─────────────┐
 │   UPGRADES  │           │  DESAFIOS   │
 └──────┬──────┘           └──────┬──────┘
        └────────────┬─────────────┘
                     ↓
              ┌──────────────┐
              │ SUBIR CARREIRA│
              └──────┬───────┘
                     ↓
                  🔁 LOOP
```

### 🧠 Progressão educacional

O jogo separa **economia** de **aprendizado**:

  Sistema        Função
  -------------- ----------------------------------------------
  💻 LOC         Recurso para upgrades e progressão econômica
  ⭐ XP          Evolução educacional e nível de carreira
  🧠 Domínio     Experiência individual em cada linguagem
  🔥 Combo Dev   Recompensa respostas corretas sem dicas
  🎯 Missões     Incentivam sessões curtas e frequentes
  🚀 Projetos    Objetivos maiores de progressão

Assim, simplesmente deixar o jogo aberto pode gerar recursos, mas o
progresso educacional também incentiva interação e resolução de
desafios.

### 💻 Tecnologias

  Tecnologia           Uso
  -------------------- ----------------------------
  HTML5                Estrutura
  CSS / Tailwind CSS   Interface e responsividade
  JavaScript           Mecânicas e lógica
  Supabase             Login e sincronização
  LocalStorage         Salvamento local
  Font Awesome         Ícones
  Web Audio API        Efeitos e batida
  Vercel               Deploy web

### 🚀 Executando localmente

Clone o projeto:

``` bash
git clone https://github.com/script33dt-glitch/Dev-game-.git
cd Dev-game-
```

Inicie um servidor local, por exemplo:

``` bash
python -m http.server 5500
```

E abra:

``` text
http://localhost:5500
```

Também é possível abrir pelo VS Code usando uma extensão de servidor
local.

> Para autenticação Google/Supabase, a URL utilizada precisa estar
> configurada entre as URLs autorizadas do projeto.

### ☁️ Contas e salvamento

O Dev Typist Pro oferece:

``` text
👤 Visitante          → progresso local
📧 E-mail + senha     → conta sincronizada
🔵 Google             → conta sincronizada
☁️ Supabase           → progresso na nuvem
```

O tutorial aparece novamente para visitantes, enquanto uma conta
autenticada registra sua conclusão para evitar repetir a introdução
desnecessariamente.

### 🔐 Segurança

A chave pública/anon do Supabase pode existir no cliente, mas **não deve
ser considerada uma camada de segurança**.

O banco deve utilizar **Row Level Security (RLS)** para garantir que
cada usuário tenha acesso somente aos próprios dados.

Nunca coloque no front-end:

``` text
❌ service_role key
❌ senhas administrativas
❌ tokens privados
❌ segredos de servidor
```

### 🗺️ Roadmap

Ideias para próximas versões:

-   [ ] mais desafios e microlições;
-   [ ] trilhas completas por linguagem;
-   [ ] revisão automática dos conteúdos com maior índice de erro;
-   [ ] projetos educacionais maiores;
-   [ ] painel avançado de estatísticas;
-   [ ] melhorias de acessibilidade;
-   [ ] navegação completa por teclado;
-   [ ] PWA instalável;
-   [ ] testes automatizados;
-   [ ] modularização de CSS e JavaScript;
-   [ ] painel para criação de conteúdos;
-   [ ] recursos opcionais para professores e turmas.

------------------------------------------------------------------------

## 🇺🇸 English

### 🎮 About Dev Typist Pro

**Dev Typist Pro** is an educational web game that combines **code
typing, programming practice, idle/clicker progression, and short logic
challenges**.

The idea is simple: open the game for a quick session, grow your virtual
developer career, and stay in frequent contact with programming concepts
and syntax.

The experience is built around three pillars:

``` text
⌨️ TYPE  →  🧠 UNDERSTAND  →  💡 SOLVE
```

Typing builds familiarity with syntax. Micro-lessons introduce concepts
in small pieces. Challenges and bug hunts encourage interpretation and
problem-solving.

> Dev Typist Pro is not intended to replace courses, documentation, or
> real development projects. It is designed as a complementary and
> entertaining practice tool.

### ✨ Features

``` text
┌──────────────────────────────────────┐
│            DEV TYPIST PRO            │
├──────────────────────────────────────┤
│  ⌨️ Code typing terminal             │
│  📈 LOC + XP + levels                │
│  🔥 Typing Combo / Dev Combo         │
│  🧠 Programming challenges           │
│  🐛 Bug hunting                      │
│  📚 Micro-lessons                    │
│  🎯 Daily missions                   │
│  🏆 Achievements                     │
│  🛒 Upgrades                         │
│  💼 Developer career                 │
│  ☁️ Cloud progress                   │
└──────────────────────────────────────┘
```

Current features include:

-   real-time code typing terminal;
-   HTML/CSS, Python, Java, PHP, SQL, and TypeScript;
-   LOC (Lines of Code) as the main game currency;
-   XP and career levels;
-   career progression from **Beginner → Intern → Junior Developer →
    Mid-level Developer → Senior Developer → Tech Lead**;
-   WPM/CPM, typing combos, and performance statistics;
-   language-specific mastery;
-   programming micro-lessons;
-   code interpretation challenges;
-   bug-hunting challenges;
-   daily missions and study streaks;
-   career projects;
-   Team, Skills, and Hardware/Software upgrades;
-   achievements;
-   server incidents and emergency deployments;
-   multiple visual themes;
-   multilingual interface;
-   sound effects and a minimal electronic background beat;
-   email/password and Google authentication;
-   guest mode;
-   local saving and Supabase cloud synchronization;
-   onboarding tutorial for new players.

### 🕹️ Gameplay loop

``` text
               ┌───────────┐
               │ TYPE CODE │
               └─────┬─────┘
                     ↓
               ┌───────────┐
               │ EARN LOC/XP│
               └─────┬─────┘
                     ↓
        ┌────────────┴────────────┐
        ↓                         ↓
 ┌─────────────┐           ┌─────────────┐
 │  UPGRADES   │           │ CHALLENGES  │
 └──────┬──────┘           └──────┬──────┘
        └────────────┬─────────────┘
                     ↓
               ┌─────────────┐
               │ LEVEL CAREER│
               └──────┬──────┘
                      ↓
                   🔁 LOOP
```

### 🧠 Learning progression

Game economy and educational progression are intentionally separated:

  System         Purpose
  -------------- -----------------------------------------------------
  💻 LOC         Currency used for upgrades and economic progression
  ⭐ XP          Educational and career progression
  🧠 Mastery     Experience in each programming language
  🔥 Dev Combo   Rewards correct answers without hints
  🎯 Missions    Encourage short and frequent sessions
  🚀 Projects    Larger progression objectives

This allows idle mechanics to remain fun without making passive resource
generation equivalent to programming mastery.

### 💻 Tech stack

  Technology           Purpose
  -------------------- --------------------------------------
  HTML5                Application structure
  CSS / Tailwind CSS   UI and responsive design
  JavaScript           Game mechanics
  Supabase             Authentication and cloud persistence
  LocalStorage         Local persistence
  Font Awesome         Icons
  Web Audio API        Sound effects and background beat
  Vercel               Web deployment

### 🚀 Run locally

Clone the repository:

``` bash
git clone https://github.com/script33dt-glitch/Dev-game-.git
cd Dev-game-
```

Start a local server:

``` bash
python -m http.server 5500
```

Then open:

``` text
http://localhost:5500
```

You can also use a local server extension in VS Code.

> Google/Supabase authentication requires the development or production
> URL to be included in the project's authorized redirect URLs.

### ☁️ Accounts and saves

``` text
👤 Guest              → local progress
📧 Email + password   → synchronized account
🔵 Google             → synchronized account
☁️ Supabase           → cloud progress
```

Guest players receive the onboarding experience on new entries, while
authenticated users keep their tutorial completion state with their
account.

### 🔐 Security

The public Supabase anon key may be present in client-side code, but it
**must not be treated as a security boundary**.

Use **Row Level Security (RLS)** to restrict each authenticated user to
their own data.

Never expose:

``` text
❌ service_role keys
❌ administrator passwords
❌ private tokens
❌ server secrets
```

### 🗺️ Roadmap

-   [ ] more challenges and micro-lessons;
-   [ ] complete learning paths for each language;
-   [ ] automatic review of frequently missed concepts;
-   [ ] larger educational projects;
-   [ ] advanced study statistics;
-   [ ] accessibility improvements;
-   [ ] full keyboard navigation;
-   [ ] installable PWA;
-   [ ] automated tests;
-   [ ] CSS/JavaScript modularization;
-   [ ] content creation dashboard;
-   [ ] optional teacher/classroom features.

------------------------------------------------------------------------

## 🤝 Contribuições / Contributing

🇧🇷 Contribuições, sugestões e testes são bem-vindos durante o
desenvolvimento. Ao alterar o projeto, preserve as mecânicas existentes,
teste visitante e login, verifique persistência e mantenha conteúdos
educacionais curtos e objetivos.

🇺🇸 Contributions, suggestions, and testing are welcome during
development. When changing the project, preserve existing mechanics,
test both guest and authenticated flows, verify persistence, and keep
educational content short and focused.

### Commits

``` text
feat: adiciona novos desafios
fix: corrige persistência do progresso
ui: melhora interface da central de estudo
docs: atualiza documentação
```

## 📂 Estrutura / Structure

``` text
Dev-game-/
├── index.html
└── README.md
```

## 👨‍💻 Autor / Author

**Arthur Pereira Bolognesi**

🇧🇷 Projeto criado para unir **programação, estudo, gamificação e
entretenimento**.

🇺🇸 A project created to combine **programming, learning, gamification,
and entertainment**.

## 📄 Licença / License

🇧🇷 A licença ainda deve ser definida. Antes de permitir redistribuição
ou contribuições externas em maior escala, adicione um arquivo
`LICENSE`.

🇺🇸 The project license has not been defined yet. Before allowing broader
redistribution or external contributions, add a `LICENSE` file.

------------------------------------------------------------------------

::: {align="center"}
### `> READY TO CODE_`

**Dev Typist Pro © 2026**

⌨️ **Type. Learn. Level up.**
:::
