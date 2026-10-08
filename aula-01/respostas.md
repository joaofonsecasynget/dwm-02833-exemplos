# Aula 1 — respostas

## Check-in (exemplo)

O portal da escola, porque mostra o horário. Há muitas respostas válidas.

## Diagnóstico

1. Em `https://www.exemplo.pt/contactos.html`: protocolo **https**; domínio **www.exemplo.pt**; página **contactos.html**.
2. Texto e títulos → **HTML**; cores e tipo de letra → **CSS**; menu que abre ao clicar → **JavaScript**.
3. **B** — cria uma ligação que abre a página `sobre.html`; «Sobre nós» é o texto clicável.
4. **B** — a página pedida não existe no servidor (o servidor respondeu, mas não encontrou o recurso).
5. Exemplos: Início, O clube, Equipas, Calendário de jogos, Notícias, Galeria, Inscrições, Contactos. Há outras respostas válidas.

## Aquecimento: do endereço à página

1. Escreves o endereço no browser.
2. O DNS devolve o endereço IP do domínio.
3. O browser envia o pedido HTTP ao servidor.
4. O servidor prepara a resposta.
5. O browser recebe os ficheiros e desenha a página.

Extensão: o nome do domínio entra no passo 2 — é ele que o DNS traduz para o endereço IP.

## Os três pilares

- Parágrafo com a história do clube → **HTML** (conteúdo e estrutura).
- Fundo da página a azul → **CSS** (apresentação).
- Mensagem que aparece ao clicar em «Enviar» → **JavaScript** (comportamento).

## Atividade: dissecar um site

Com o `exemplo.html` desta pasta (abre-o com o Live Server e carrega em F12):

- **Etiquetas (Elements)**: `h1`, `p`, `a`, `img`, `ul`/`li`, `nav`, `footer`.
- **Regras CSS (Styles)**: `font-family: Arial, sans-serif;`, `color: navy;`, `background-color: #eeeeee;`.
- **Alteração ao vivo**: mudar `color: navy` para `color: red` no painel Styles — o título fica vermelho até recarregar a página.
- **JavaScript (Sources)**: o ficheiro `exemplo.js`; ao clicar no botão aparece «Inscrições abertas!».

Num site público as evidências são outras; vale ligar o que observaste aos três pilares.

## Preparar o ambiente

A pasta do projeto tem `index.html`, `css/`, `js/` e `img/` — ver a pasta `projeto/` deste repositório.
