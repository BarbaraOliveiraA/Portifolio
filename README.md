# Portfólio Profissional - Barbara de Oliveira
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![BOOTSTRAP](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

## Descrição do portfólio
Site de portfólio profissional e acadêmico desenvolvido para apresentar minha trajetória, competências técnicas, principais projetos realizados e canais de contato na área de desenvolvimento de sistemas.

## Tecnologias utilizadas
- HTML5: Estruturação semântica das páginas.
- SS3: Estilizações customizadas e efeitos visuais.
- Bootstrap 5.3: Framework CSS para responsividade, grid system, cards, carrossel e barra de navegação.
- Devicon: Biblioteca de ícones para tecnologias e ferramentas.
- Imagens locais organizadas em diretório próprio (/imagens)

## Conteúdo da Página

O site foi construído como uma página única (one-page) com navegação por âncoras. O menu superior fixo permite navegar entre as seções Perfil, Projetos e Contato, e o nome no canto esquerdo do menu leva de volta ao topo, onde fica o carrossel. O design é responsivo, adaptando-se a telas de computadores, tablets e smartphones graças ao sistema de grades do Bootstrap.

|Seção | Conteúdo |
|---|---|
|Carrossel | Três imagens de destaque com transição em fade |
|Perfil | Foto, apresentação, cards de informações (Localização, Área de interesse, Formação e Objetivo) e as tecnologias e ferramentas (HTML5, CSS3, Bootstrap, Python, GitHub e VS Code) |
|Projetos |	Três cards: Portfólio Pessoal, Sistema em Python e Página Web Responsiva |
|Contato | Botões de e-mail, GitHub e LinkedIn, além da localização |


## Descrição do recurso novo adicionado
Como recurso avançado junto do modelo base visto em sala de aula, foi implementado:
1. Carrossel com efeito fade e padronização de imagens: Utilização de transições suaves de desvanecimento (carousel-fade) combinadas com regras de CSS (object-fit: cover) para garantir que as imagens do carrossel e dos cards mantenham uma proporção uniforme, sem distorções.
2. Integração de ícones vetoriais (Devicon): Seção de competências com os logotipos das linguagens e ferramentas estudadas.
3. Cards com alinhamento flexível e flexbox: Uso de utilitários do Bootstrap (h-100, d-flex flex-column) para manter a uniformidade visual dos elementos independentemente da quantidade de texto.
4. Efeito de zoom nos cards de projetos: Ao passar o mouse sobre um card, ele aumenta levemente e ganha uma sombra mais forte, com transição suave.
5. Botão "voltar ao topo": Botão fixo no canto inferior direito que fica invisível no topo da página e aparece gradualmente conforme a página é rolada.

## Explicação de como recursos foram implementados
Os recursos visuais foram implementados no arquivo externo Estilo.css, ligado ao index.html depois do CSS do Bootstrap:

1. A classe .carousel-item img fixa uma altura padrão de 500px e utiliza a propriedade object-fit: cover para recortar proporcionalmente as imagens.
2. A classe .project-img aplica o mesmo comportamento de redimensionamento nas fotos dos projetos.
3. A classe .profile-img define o tamanho da foto de perfil (220px por 220px), também com object-fit: cover.
4. A classe .project-card usa transition e a pseudoclasse :hover com transform: scale(1.05) para criar o efeito de zoom nos cards.
5. O botão "voltar ao topo" (#btnTopo) é um link posicionado com position: fixed. Para aparecer só depois de rolar a página, foi usada uma animação controlada pela rolagem (animation-timeline: scroll()), que deixa o botão transparente nos primeiros 200px e totalmente visível a partir de 300px. Em navegadores que não suportam esse recurso, o botão fica sempre visível, e continua funcionando.

## Link do site publicado
https://barbaraoliveiraa.github.io/Portifolio/

## Como executar o projeto
1. Faça o download deste repositório para o seu computador.
2. Certifique-se de manter a pasta imagens e o arquivo Estilo.css no mesmo diretório do arquivo index.html.
3. Dê dois cliques no arquivo index.html para abri-lo em qualquer navegador (Chrome, Firefox, Edge, etc.). É necessário estar conectado à internet, pois o Bootstrap e o Devicon são carregados por CDN.