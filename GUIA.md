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
2. Usa o **email da escola** (`…@aelousada.net`) e uma palavra-passe forte, só tua.
3. Escolhe um username que te identifique (por exemplo `nome-apelido`), sem alcunhas.
4. Resolve a verificação e escreve o código que recebes no email da escola.

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

No VS Code, **Terminal → New Terminal**, e escreve, uma linha de cada vez (com o teu nome e o teu email):

```
git config --global user.name "Nome Apelido"
git config --global user.email "numero@aelousada.net"
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

## 8. Quando corre mal

| O que aparece | O que fazer |
|---|---|
| `Please tell me who you are` / `Author identity unknown` | Faz a parte 5. |
| `Updates were rejected because the remote contains work…` | Faz **Pull** e depois **Sync Changes**. |
| `Merge` ou ficheiros com conflito (**C**) | Não apagues nada: chama o professor. |
| O VS Code pede para iniciar sessão | Inicia sessão no GitHub com a **tua** conta. |
| `Repository not found` / `Permission denied` | Confirma que estás com a tua conta e no teu repositório. |
| O ficheiro não aparece no GitHub | Faltou o commit ou o push: vê o painel e faz **Sync Changes**. |
| O ficheiro está na pasta errada | Arrasta-o no explorador do VS Code para a pasta certa, commit e Sync Changes. |

## 9. Verificação final

- [ ] A conta do GitHub usa o email da escola.
- [ ] O repositório chama-se `dwm-02833`, é privado e o professor é colaborador.
- [ ] `git config --global --list` mostra o teu nome e o teu email.
- [ ] O VS Code tem as extensões da disciplina.
- [ ] Fizeste um commit de teste e vês a tua mensagem no GitHub.

Este repositório (`dwm-02833-exemplos`) tem os exemplos das aulas, organizados como o teu. Podes copiá-los; o que conta é perceberes o código.
