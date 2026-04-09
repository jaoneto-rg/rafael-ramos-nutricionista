# Rafael Ramos | Nutricionista - Landing Page

Esta documentação resume as escolhas de design e a estrutura de arquitetura criadas para a Landing Page do Rafael Ramos. O objetivo foi construir uma experiência fluída e moderna voltada para conversão de modo autêntico.

## 🎨 Sistema de Design e Identidade Visual

A paleta de cores e tipografia foram pensadas para afastar a página da "frieza clínica" tradicional de saúde e abraçar um tom de bem-estar orgânico e moderno.

- **Cores Principais:**
  - `Emerald Pine (#084734):` Verde profundo usado como espinha dorsal da leitura. Transmite maturidade e serenidade.
  - `Lime Glow (#CEF17B):` Verde vibrante/lima usado de forma pontual para *Call To Actions (CTAs)*, destaques e elementos interativos.  
  - `Green Tea (#CDEDB3):` Verde pálido usado no plano de fundo. Ele assume o lugar do branco tradicional, diminuindo a fadiga visual e reforçando o conceito "orgânico".
  - `Deep Dark (#021f17):` Verde super fechado para separar o rodapé.

- **Tipografia:**
  - **Títulos:** `Playfair Display` (Serifada) - traz elegância, profissionalismo e confiabilidade; evocando autoridade.
  - **Corpo do texto:** `DM Sans` (Sem serifa) - garante leitura limpa, minimalista e altíssima legibilidade em dispositivos móveis.

---

## Estrutura e Escolhas por Seções

### 1. Navegação Lateral Fixa
Fugindo do padrão de um menu presencial simples no topo, a página utiliza uma navegação fixa lateral flutuante por ícones no desktop (com tooltips reveladoras).
*No celular, ela se transforma fluidamente para uma barra fixa no rodapé estilo "aplicativo nativo", favorecendo a usabilidade onde o polegar naturalmente descansa.*

### 2. Home (Hero Section)
A tela de entrada foca no WOW-factor inicial. Um gradiente sutil com textura de "ruído" preenche o fundo de forma leve. Textos contam com animações em cascata usando `IntersectionObserver` e o design dá dois caminhos de CTAs imediatos bem direcionados num layout agradável tipo grade.

### 3. Sobre
Um design orgânico de *Grid* separa as fotos do texto. Para organizar os dados curriculares de modo dinâmico, criamos "Info Cards" usando ícones com visual glassmórfico (sobreposição translucida com sombras projetadas), removendo enormes blocos de texto tediosos.

### 4. Minha Jornada
Seção concebida sem estourar o limite da parte de baixo dos monitores de tamanho padrão (com uma altura mínima preenchida na horizontal e espaçamentos contidos). Organizada em formato de um carrossel horizontal de *cards* modernos que mostram estágios e projetos profissionais sem criar poluição de texto no scroll natural.

### 5. Receitas Favoritas
Construída com **Glassmorphism**. Os cards possuem um fundo de cor branca difusa em ambiente claro (`rgba(255, 255, 255, 0.6)`) que levitam quando ganham "hover" no mouse. O grande diferencial dessa seção não é apenas mostrar a receita, e sim os Modais Popups customizados com dicas do nutricionista, acionados via click.

### 6. Contato
Exibe as credenciais importantes em cartões verdes densos minimalistas de 4 colunas para alta assimilação com um enorme botão central super-convidativo flutuando focado em direcionar para o *WhatsApp*.

### 7. Depoimentos & Footer
Mais um formato em carrossel auto-rotativo (anima-se automaticamente). Isso traz provas sociais dinâmicas sem ocupar longos espaços na tela.  
A página é fechada num rodapé simples texturizado mais escuro simulando *Dark Mode* para selar a elegância e contrastar todas as redes sociais.

---

## ✨ Tecnologias Usadas
- Todo o design foi concebido em **Vanilla HTML, CSS e JS Puro** sem uso pesado de frameworks externos de visualização para prover renderização absolutamente imediata, altíssima customização sobre o layout responsivo e SEO perfeitamente polido.
- Animações usando `@keyframes`, Easing suave de scroll matemático com JavaScript nativo e estrutura com Flexbox / CSS Grid.
