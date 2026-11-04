# Portefólio Marta Sousa

Site estático em HTML e CSS, sem dependências nem processo de build. Pronto para o GitHub Pages: os ficheiros ficam na raiz do repositório.

## Páginas
- `index.html`: início (projetos selecionados, índice com filtro, sobre, contacto)
- `experiencia-profissional.html`: material comercial, website, redes sociais, fotografia
- `trabalhos-academicos.html`: dissertação, projetos, desenho, filmes, concurso
- `interesses.html`: fotografia, faup fest, trabalhos manuais, design
- `a-margem-do-rio.html`: página da dissertação
- `404.html`: página de erro

## Pastas
- `css/estilo.css`: todos os estilos. As cores, o degrau da cascata (`--degrau: 4ch`) e os espaçamentos estão no `:root`, no topo.
- `img/`: imagens. `ficheiros/`: documentos para descarregar (cv).

## Como funciona o layout
- Cascata: as classes `d1` a `d4` recuam uma linha 1 a 4 degraus.
- Pontos: `<span class="ponto p44 vermelho">`; o tamanho vem de `p10`, `p12`, `p16`, `p26`, `p36` ou `p44` e a cor de `vermelho`, `lilas`, `azul`, `rosa`, `amarelo`, `verde` ou `verde-claro`.
- Composições desencontradas: cada `.bloco` recebe `--w` (largura), `--y` (desfasamento vertical) e `--x` (recuo). Em grelhas, cada item pode receber `--y`. No telemóvel (até 760px) os desfasamentos desaparecem.
- Índice da página inicial: cada linha tem `data-area` (arquitectura, comunicacao, design, fotografia, manuais) e `--n` (degrau). O filtro está no fim do `index.html`.

## Imagens
As caixas cinzentas com texto entre [ ] são lugares para imagens. Para pôr uma fotografia, mantém a caixa (guarda a proporção) e acrescenta lá dentro, por exemplo:

    <div class="imagem" style="--r: 4 / 3"><img src="img/lioz-01.jpg" alt="Descrição da imagem" loading="lazy"></div>

e retira o texto entre [ ]. Convém exportar as imagens em JPG com cerca de 2000px no lado maior e menos de 500 KB.

## Sistema visual
- Letra: Source Code Pro (Google Fonts), 400 e 700
- Fundo #F0EDE5, texto #19181A, texto secundário #5C5A59, caixas de imagem #E4E0D6
- Pontos: vermelho #EF3728, lilás #A289CC, azul #344CA5, rosa #F24AAB, amarelo #F4D717, verde #4DC071, verde-claro #ABDE83
- Só círculos; sem cantos arredondados, sombras, gradientes ou linhas divisórias
