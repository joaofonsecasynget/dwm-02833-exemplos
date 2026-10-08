# Guia da turma 10ºDS — Desenvolvimento Web e Móvel

Instruções para preparares o teu computador e o teu repositório da **UC02833 Conceber aplicações para a web na vertente frontend**. Faz os passos pela ordem e só avances quando vires o resultado esperado.

> **Regras em todas as aulas:** todo o teu trabalho fica no teu repositório do GitHub e a entrega é o **commit e o push**, feitos no VS Code — não há entregas no Teams. Antes de começares, fazes sempre **pull** (ou Sync Changes).

## O teu repositório

- Nome: **`dwm-02833`** (exatamente assim, em minúsculas), **privado**, com README.
- Colaborador: o professor, utilizador **`joaofonsecasynget`**.
- Onde o clonas no computador: a pasta **Documentos**.
- Organização:
  - `projeto/` — o site do Projeto Web: `index.html`, `css/`, `js/` e `img/`
  - `fichas/` — as fichas do Projeto Web (Word e PowerPoint): ficha 0, ficha 1, wireframes, …

```
dwm-02833/
  README.md
  projeto/
    index.html
    css/
    js/
    img/
  fichas/
    Ficha 1 - <nome do projeto>.docx
    Wireframes - <nome do projeto>.pptx
```

Nomes sempre sem espaços, sem acentos, em minúsculas, e com o número da aula com dois algarismos (`aula-03`, não `aula3` nem `Aula 3`).

## 1. Criar a conta no GitHub

1. Abre `https://github.com/signup`.
2. Usa um **email pessoal a que tenhas acesso** — **não** o email da escola (`…@aelousada.net`), porque não tens acesso a ele e não receberias o código de verificação, os convites nem os avisos do GitHub. Escolhe uma palavra-passe forte, só tua.
3. Escolhe um username no formato **`nome-apelido`** (por exemplo `ana-silva`), sem alcunhas, para os professores te identificarem.
4. Resolve a verificação e escreve o código que recebes nesse email.

**Já tens conta com o email da escola?** Fotografia (canto superior direito) → **Settings** → **Emails** → **Add email address** → o teu email pessoal (confirma-o com a mensagem que recebes) → em **Primary email address**, escolhe-o. Se o username não estiver no formato `nome-apelido`: **Settings** → **Account** → **Change username** (os repositórios e o acesso do professor mantêm-se).

**Resultado esperado:** estás na página inicial do GitHub, com o teu username no canto superior direito.

## 2. Criar o repositório `dwm-02833`

1. No GitHub, **+** (canto superior direito) → **New repository**.
2. Repository name: `dwm-02833`. Escolhe **Private** e marca **Add a README file**. **Create repository**.
3. **Settings** → **Collaborators** → **Add people** → `joaofonsecasynget` → **Add … to this repository**.

**Resultado esperado:** o repositório tem o cadeado (privado) e o professor aparece em Collaborators.

## 3. Instalar o Git

- **Windows:** descarrega em `https://git-scm.com/download/win` e aceita as opções marcadas, exceto: em *default editor* escolhe **Visual Studio Code**; em *initial branch* escolhe **Override** com `main`.
- **Sem administrador (computadores da escola):** usa o **Portable Git** (mesma página), extrai-o para a tua pasta de utilizador e, no VS Code, em Definições, põe em `git.path` o caminho de `cmd\git.exe`.
- **macOS:** no Terminal, `git --version`; se pedir, instala as ferramentas de linha de comandos.

**Resultado esperado:** `git --version` mostra `git version 2.x.x`.

## 4. Instalar o VS Code e as extensões

1. Descarrega em `https://code.visualstudio.com` (no Windows, o **User Installer**, com **Add to PATH**).
2. No VS Code, **Ctrl+Shift+X** (Mac: **Cmd+Shift+X**) e instala:
   - **Live Server** (Ritwick Dey)

**Resultado esperado:** as extensões aparecem em Extensões → Installed.

## 5. Configurar o Git (uma vez por computador)

No VS Code, **Terminal → New Terminal**, e escreve, uma linha de cada vez (com o teu nome e o email da tua conta do GitHub):

```
git config --global user.name "Nome Apelido"
git config --global user.email "o-teu-email-pessoal@exemplo.pt"
git config --global init.defaultBranch main
```

Confirma com `git config --global --list`. **Num computador partilhado da escola**, confirma no início de cada aula que o nome e o email são os teus: se não forem, os teus commits ficam com o nome de um colega.

## 6. Clonar o repositório no VS Code

1. **Ctrl+Shift+P** → `Git: Clone` → **Clone from GitHub**; na primeira vez, inicia sessão no GitHub e autoriza.
2. Escolhe `teu-username/dwm-02833` e a pasta: a pasta **Documentos**.
3. **Open**. Cria as pastas da organização acima com **New Folder**, no explorador do VS Code.

**Resultado esperado:** o explorador do VS Code mostra o repositório, o README.md e as tuas pastas.

## 7. O ciclo de trabalho, sempre no VS Code

1. **Pull antes de começar:** painel **Controlo de código-fonte** (**Ctrl+Shift+G**) → **…** → **Pull** (ou **Sync Changes**).
2. **Trabalha** e guarda com **Ctrl+S**. Os ficheiros alterados aparecem no painel com **M** (modificado) ou **U** (novo).
3. **Commit:** escreve na caixa **Message** o que fizeste (por exemplo `Aula 5: estrutura semântica da página inicial`) e carrega em **Commit** (✓); se perguntar pelo *stage*, responde **Yes**.
4. **Push:** carrega em **Sync Changes**.
5. **Confirma no GitHub** que os ficheiros e a tua mensagem lá estão.

- Para ver o site: abre `projeto/index.html` no VS Code e carrega em **Go Live** na barra de baixo (Live Server).
- O Projeto Web é feito a pares: cada aluno tem o seu repositório, com o trabalho do par.

## 8. Em todas as aulas, num computador da escola

Os computadores da sala são partilhados: o que ficou da aula anterior pode ser de um colega. Faz sempre esta rotina — com prática, demora menos de 5 minutos no início e 5 no fim.

### No início da aula

1. **O Git está instalado?** No VS Code, **Terminal → New Terminal**, escreve `git --version`.
   - Resultado esperado: `git version 2.x.x`. Se aparecer `git is not recognized`, faz a parte 3 (Portable Git).
2. **O nome e o email são os teus?** Escreve `git config --global --list`.
   - Se `user.name` ou `user.email` não forem os teus (ou não aparecerem), escreve:
     ```
     git config --global user.name "Nome Apelido"
     git config --global user.email "o-teu-email-pessoal@exemplo.pt"
     ```
   - Resultado esperado: `git config --global --list` mostra o teu nome e o teu email.
3. **A sessão do GitHub é a tua?** No VS Code, clica no ícone **Contas** (canto inferior esquerdo). Se aparecer a conta de outra pessoa, **Sign Out** dessa conta.
4. **Clona o teu repositório:** **Ctrl+Shift+P** → `Git: Clone` → **Clone from GitHub** → inicia sessão com a **tua** conta → `teu-username/dwm-02833` → pasta **Documentos** → **Open**.
   - Se a pasta `dwm-02833` já existir em Documentos, abre-a (**File → Open Folder**) e faz **Pull** em vez de clonar.
   - Resultado esperado: o explorador do VS Code mostra o teu repositório, com o trabalho das aulas anteriores.

### Durante a aula

5. Trabalha no VS Code (código) ou no Word/PowerPoint (fichas), **sempre dentro da pasta `dwm-02833`** em Documentos, e guarda (**Ctrl+S**).
   - Um ficheiro do Office aberto a partir do Teams ou do OneDrive não fica no repositório: usa **Ficheiro → Guardar uma cópia** e escolhe a pasta `dwm-02833/fichas` em Documentos.

### No fim da aula

6. **Commit e push** (parte 7): mensagem que diga o que fizeste, **Commit** (✓) e **Sync Changes**.
7. **Confirma no GitHub**, no browser, que o teu commit lá está, com a tua mensagem.
8. **Termina a sessão**, para o colega seguinte não usar a tua conta:
   - VS Code: ícone **Contas** → a tua conta do GitHub → **Sign Out**;
   - Windows: **Gestor de Credenciais** (procura no menu Iniciar) → **Credenciais do Windows** → remove as entradas `git:https://github.com` e `GitHub` (se existirem);
   - browser: termina a sessão no GitHub.
9. **Apaga a pasta `dwm-02833` de Documentos**, depois de confirmares o push — na próxima aula clonas de novo.

> **Porquê tudo isto?** Se a sessão ou o nome de um colega ficarem no computador, o teu trabalho vai para o repositório dele, ou fica com o nome dele, e conta como não entregue.

## 9. Quando corre mal

| O que aparece | O que fazer |
|---|---|
| `Please tell me who you are` / `Author identity unknown` | Faz a parte 5. |
| O commit aparece no GitHub com o nome de um colega | O nome e o email do Git eram de outra pessoa: faz o passo 2 da parte 8 antes do próximo commit. |
| O push foi para o repositório de um colega, ou dá `Permission denied` com o username de outra pessoa | A sessão do GitHub era de outra pessoa: faz o passo 8 da parte 8 (terminar sessão) e volta a clonar com a tua conta. |
| `Updates were rejected because the remote contains work…` | Faz **Pull** e depois **Sync Changes**. |
| `Merge` ou ficheiros com conflito (**C**) | Não apagues nada: chama o professor. |
| O VS Code pede para iniciar sessão | Inicia sessão no GitHub com a **tua** conta. |
| `Repository not found` / `Permission denied` | Confirma que estás com a tua conta e no teu repositório. |
| O ficheiro não aparece no GitHub | Faltou o commit ou o push: vê o painel e faz **Sync Changes**. |
| O ficheiro está na pasta errada | Arrasta-o no explorador do VS Code para a pasta certa, commit e Sync Changes. |

## 10. Verificação final

- [ ] A conta do GitHub usa um email pessoal a que tens acesso e o username está no formato `nome-apelido`.
- [ ] O repositório chama-se `dwm-02833`, é privado e o professor é colaborador.
- [ ] `git config --global --list` mostra o teu nome e o teu email.
- [ ] O VS Code tem as extensões da disciplina.
- [ ] Fizeste um commit de teste e vês a tua mensagem no GitHub.

Este repositório (`dwm-02833-exemplos`) tem os exemplos das aulas, organizados como o teu. Podes copiá-los; o que conta é perceberes o código.
