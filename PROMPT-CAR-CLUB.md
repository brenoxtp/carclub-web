# PROMPT MESTRE — CAR CLUB CENTRO AUTOMOTIVO
## Esqueleto de landing page | direção de arte Future Industrial + CRO

Você é um **diretor de arte digital, engenheiro front-end sênior e estrategista de conversão**. Desenvolva a estrutura visual e textual de uma landing page para a **Car Club Centro Automotivo**, Três Pontas–MG.

**Objetivo exclusivo:** transformar visitantes em pedidos qualificados de avaliação/orçamento pelo WhatsApp.

**Resultado desejado:** uma experiência de marca automotiva contemporânea, com acabamento de nível premium, estrutura editorial forte e linguagem direta. Visual **futurista industrial refinado**, inspirado em design automotivo, painéis de precisão, fotografia de estúdio e arquitetura de alta performance. **Não é cyberpunk, neon, gamer, concessionária de supercarros ou template genérico de oficina.**

Nesta fase, criar **o esqueleto do site**: hierarquia, componentes, layout mobile/desktop, copy de trabalho, inventário de imagens e design tokens. Se houver solicitação para codificar, implementar fielmente a estrutura aprovada, sem inventar novas seções.

### Referências e fonte da verdade
- Oficina e fotos reais: https://www.google.com/maps/place/Car+Club+Centro+Automotivo/
- Site oficial: https://www.oficinacarclubtp.com.br/
- Instagram: https://www.instagram.com/oficinacarclub/
- Metodologia UI UX Pro Max: https://github.com/nextlevelbuilder/ui-ux-pro-max-skill
- Repositório do projeto: https://github.com/brenoxtp/carclub-web

**Ordem de autoridade:** informação factual e identidade da Car Club > materiais oficiais > recomendações da skill > preferências estéticas genéricas.

### 1. Procedimento da skill UI UX Pro Max
1. Verifique se a skill realmente existe no ambiente. Como o projeto foi reiniciado, **não presuma que ela esteja instalada**. Se não estiver, instale conforme a documentação oficial ou consulte as orientações de referência, deixando clara a limitação.
2. Leia \`.claude/skills/ui-ux-pro-max/SKILL.md\` e \`references/quick-reference.md\` quando disponíveis.
3. Se o script existir, execute, a partir da raiz do projeto:
   \`python .claude/skills/ui-ux-pro-max/scripts/search.py "premium automotive bodywork local service high conversion" --design-system -p "Car Club Centro Automotivo"\`
4. Consulte \`--domain landing\` para composição e fluxo de prova → CTA; \`--domain ux\` para acessibilidade/interação; \`--domain typography\` para hierarquia; \`--stack html-tailwind\` somente se for o stack identificado.
5. Registre as conclusões relevantes. **A skill orienta decisões; não autoriza ignorar o briefing nem inventar dados comerciais.**

## 2. DNA visual — FUTURE INDUSTRIAL

Imagine uma instalação automotiva premium: grafite fosco, iluminação recortada, reflexos controlados na pintura, superfícies precisas e sinalização funcional. Transfira essa linguagem para o layout **sem imitar um painel de automóvel literalmente**.

**Paleta proposta, sujeita à validação com o logotipo real:**
- Base profunda: \`#0B0E11\` — Hero, Header, Footer.
- Grafite estrutural: \`#151A1F\` — containers de conteúdo.
- Metal escuro: \`#222A30\` — planos elevados e divisórias.
- Borda técnica: \`#343D43\` — linhas finas, discretas.
- Branco suave: \`#F3F5F5\` — headlines e texto principal.
- Cinza claro: \`#B6BEC3\` — apoio com contraste adequado.
- Laranja de ação: **amostrar do logotipo oficial**; o exemplo \`#F47729\` é provisório e não deve substituir a cor confirmada da marca.

**Tipografia:**
- Headline: família sans **condensada, firme e geométrica**, por exemplo Barlow Condensed ou equivalente comprovadamente adequado à identidade; peso 600–700, sem exagerar em CAIXA ALTA.
- Corpo/menus: sans contemporânea altamente legível (ex.: Manrope), 16–18 px, line-height 1,5–1,65.
- Display H1: \`clamp(2.6rem, 5.4vw, 5.25rem)\`, até ~10 palavras por linha visual; no mobile, quebras controladas.
- Headlines de seção: \`clamp(2rem, 3.8vw, 3.7rem)\`; texto nunca minúsculo nem acinzentado demais.
- Destaque por peso, escala e composição, **não por textos em gradiente**.

**Grid e geometria:**
- Container máximo ~1280 px, gutters de 24 px mobile / 40–64 px desktop.
- 4 colunas mobile; 12 colunas desktop. Seções com ritmos diferentes, mas alinhadas ao mesmo grid.
- Espaçamento vertical entre seções ~88–128 px desktop e 56–80 px mobile.
- Bordas 1 px e raios **contidos (8–14 px)**; evitar cartões inflados ou todos com a mesma dimensão.
- Clima futurista construído com **alinhamento técnico, assimetria controlada, foto grande, recortes editoriais, contraste material e microinterações** — nunca com sobreposição gratuita de “glassmorphism” e brilhos fluorescentes.

## 3. Design de botões — substituir a aparência genérica

Crie um pequeno **sistema de CTA** coerente em toda a página.

**Primário — Solicitar orçamento**
- Altura desktop 54–58 px; mobile mínimo 52 px, largura total quando necessário.
- Laranja sólido com texto escuro de contraste verificado; borda nítida; raio 10 px.
- Rótulo explícito: **“Solicitar avaliação pelo WhatsApp”**.
- Ícone vetorial discreto de seta avançando à direita; a seta não pode tomar mais atenção que a ação.
- Hover desktop: leve mudança de luminosidade + deslocamento da seta 3–4 px em ~180 ms; focus visível de 2 px e contraste AA; active com feedback de pressão sem saltos no layout.
- Não usar brilho neon, sombra pulsante, gradiente chamativo, “faça já” ou falsa urgência.

**Secundário — Explorar conteúdo**
- Fundo transparente, borda técnica fina, texto claro, altura e raio iguais ao primário.
- Exemplos: “Ver nossos serviços”, “Conhecer o processo”, “Como chegar”.
- Hover: preenchimento grafite + borda sutilmente mais clara; preservar foco e contraste.

**CTA contextual nos serviços**
- Link textual de ação **“Pedir avaliação deste serviço”** com seta vetorial.
- Área de toque ≥44 px e estados hover/focus definidos; não colocar quatro botões enormes idênticos em sequência.

**Sticky mobile**
- Barra compacta fixa no rodapé com um CTA principal, respeitando safe-area. Só aparece após o visitante passar pelo primeiro CTA do Hero e **não deve cobrir FAQ, mapa ou footer**.

## 4. Arquitetura dos containers — fugir dos cards prontos

**Não montar a landing page com uma pilha de retângulos arredondados iguais.** Trate cada seção como uma composição própria:

- **Hero editorial:** coluna de texto ~42% e imagem real ~58% no desktop. Imagem com proporção cinematográfica, corte consciente, enquadramento preservando carro/oficina. Sobre a imagem, no máximo uma tarja funcional com informação **verificada**, nunca números fictícios. No mobile, headline → texto → CTA → foto.
- **Serviços em mosaico assimétrico:** bloco principal de pintura/funilaria maior e 2–3 blocos menores para as demais soluções, ou pares 7/5 e 5/7. Cada tile tem imagem, degradê apenas quando necessário para legibilidade e texto sobre superfície sólida ou overlay contrastante. Não superlotar.
- **Detalhe e acabamento:** seção split-screen com **fotografia close dominante (55–60%)** e coluna de copy curta. Uma linha fina serve de referência visual, não decoração.
- **Processo e técnica:** seção oposta à anterior, com imagem de profissional em ação ou ferramenta em contexto real, seguida de etapas **somente se verificadas**. A composição deve sugerir precisão, não parecer um SaaS dashboard.
- **Galeria de trabalhos:** uma fotografia destaque ampla + miniaturas em grid editorial; usar fotos reais identificadas e autorizadas. Sem carrossel automático.
- **Sobre / diferencial:** imagem humana de fachada/equipe + bloco de texto com respiro; menos cartões, mais presença editorial.
- **FAQ / local:** painéis bem estruturados, linhas divisórias discretas, interações acessíveis e mapa com proporção reservada.

**Sistema de superfícies:** alternar faixas de fundo profundo e grafite, com seções de foto em largura ampla e limites de conteúdo consistentes. As superfícies devem orientar o olhar, não parecer caixas flutuando aleatoriamente.

## 5. Direção de copy — menos clichê, mais autoridade visual

Falar como uma **empresa automotiva segura do próprio trabalho**, não como anúncio apelativo. Frases curtas, concretas e com ritmo. Em cada seção: **1 mensagem principal + 1 explicação enxuta + 1 ação quando fizer sentido**.

**Proibir:** “somos apaixonados pelo que fazemos”, “qualidade incomparável”, “transforme sua experiência”, “soluções inovadoras”, “equipe altamente capacitada” sem prova, “a melhor oficina”, contadores e depoimentos inventados, escassez falsa.

### Copys orientadoras — usar ou refinar sem mudar o significado

**Hero**
- H1: **“Seu carro merece precisão em cada detalhe.”**
- Apoio: “Funilaria, pintura e estética automotiva em Três Pontas. Um atendimento claro para quem valoriza o resultado do próprio carro.”
- CTA: **“Solicitar avaliação pelo WhatsApp”**
- CTA secundário: “Conhecer os serviços”

**Serviços**
- Título: **“O serviço certo para cada detalhe do seu carro.”**
- Apoio: “Da recuperação da carroceria ao acabamento da pintura, encontre o cuidado que seu veículo precisa.”
- Tiles: “Pintura automotiva” / “Funilaria e reparos” / “Polimento e estética” / “Reparos de seguradora”. Descrições com 1–2 frases específicas baseadas em serviços oficiais.

**Seção hoje chamada “Acabamento que aparece de perto.”**
- Título substituto: **“A diferença aparece nos detalhes.”**
- Apoio: **“Uniformidade, brilho e cuidado com cada superfície. É de perto que o acabamento revela sua qualidade.”**
- Imagem prioritária: **close real de pintura, polimento ou acabamento**. Se usar ilustração do site oficial, não rotular como trabalho executado pela oficina.
- Container: foto large 60% / copy 40%; detalhe técnico discreto; zero cartões de ícone.

**Seção hoje chamada “O cuidado que cada etapa do reparo exige.”**
- Título substituto: **“O resultado começa antes do acabamento.”**
- Apoio: **“Avaliar, reparar e finalizar exigem atenção em momentos diferentes do serviço. Cada etapa tem sua importância.”**
- Imagem prioritária: profissional real executando serviço, bancada/equipamentos ou foto real do processo de funilaria/pintura; a **foto de colisão não representa o processo em andamento**.
- Container: layout inverso ao acabamento; se não houver fotos verificadas de execução, criar slot visual sem inventar profissional ou procedimento.

**Trabalhos realizados**
- Título: **“O acabamento fala por si.”**
- Apoio: “Veja registros reais dos serviços realizados pela Car Club.” *Exibir somente com comprovação visual; se ainda não tiver fotos, substituir por seção em preparação no esqueleto, não afirmar que as fotos são trabalhos reais.*
- Galeria de uma peça destacada + conjunto de imagens menores.

**Diferenciais / Sobre**
- Título: **“Detalhe no serviço. Clareza no atendimento.”**
- Apoio: “Conheça a estrutura e a forma de trabalho da Car Club.” Conteúdo subsequente deve vir do site oficial e de materiais autorizados.

**FAQ**
- Título: **“Suas dúvidas, respondidas sem rodeios.”**
- Perguntas sobre avaliação, tipo de reparo, pintura e seguradoras. Responder apenas com procedimentos verificados.

**CTA final**
- Título: **“Vamos entender o que seu carro precisa?”**
- Apoio: “Fale com a Car Club e explique o serviço que você procura.”
- CTA: **“Conversar sobre meu veículo”** (abre WhatsApp com mensagem contextual).

## 6. Imagens reais — cada imagem tem um papel estratégico

Inspecione a foto **antes** de associar a qualquer copy. Priorize Google Maps, Instagram autorizado e site oficial. Não confundir imagens editoriais/ilustrativas com provas de trabalhos concluídos.

**Materiais a verificar e classificar:**
- Logotipo: https://d4polyhz8pjtz.cloudfront.net/6269/cor1logo21-20240722130726.png
- Banner institucional: https://d4polyhz8pjtz.cloudfront.net/6269/paraquemvalorizacadadetalhedoseucarro-20240723150220.png
- Ilustração de polimento: https://d4polyhz8pjtz.cloudfront.net/6269/quero-saber-mais-20240716155658_400.png
- Ilustração de acabamento: https://d4polyhz8pjtz.cloudfront.net/6269/quero-saber-mais-20240716155734_400.png
- Ilustração de colisão/funilaria: https://d4polyhz8pjtz.cloudfront.net/6269/quero-saber-mais-20240716155626_400.png

**Matriz de decisão:**
- Fachada real: hero alternativo, “Sobre”, localização → **prova de existência**.
- Equipe real em serviço: seção de processo → **confiança na execução**.
- Close real de pintura/polimento: seção “A diferença aparece nos detalhes” → **prova sensorial do acabamento**.
- Veículo concluído com origem identificada: galeria → **evidência de resultado**.
- Carro acidentado: card de funilaria → **identificação do problema**, nunca “depois”.
- Banner promocional: apoio institucional se a composição permitir; **não apresentar como registro de serviço**.

Cada imagem deve receber legenda interna na documentação com **URL, conteúdo realmente visto, seção, função de conversão, responsável e situação da autorização**. Se não puder confirmar origem/licença, deixe placeholder sinalizado, sem foto gerada ou falsa.

## 7. Hierarquia final — manter esta ordem no mobile e desktop

1. **Header** — logo, menu enxuto, CTA de avaliação.
2. **Hero** — proposta objetiva + fotografia real + CTA.
3. **Serviços** — mosaico editorial de 4 soluções e CTAs contextuais.
4. **Detalhe / acabamento** — foto macro dominante + copy “A diferença aparece nos detalhes”.
5. **Processo / reparo** — fotografia de execução real + copy “O resultado começa antes do acabamento”.
6. **Trabalhos realizados** — galeria de evidência real, se disponível.
7. **Diferenciais e Sobre** — estrutura/equipe reais, história e atendimento.
8. **Avaliações + FAQ** — somente avaliações verificadas; dúvidas essenciais.
9. **Localização e CTA final** — mapa/rotas, contato, chamada de orçamento.
10. **Footer** — identidade, links e informações verificadas.

*Contato divulgado no site oficial:* (35) 99954-1742. *Endereço:* Rua José Carlos Andrade, 205, Três Pontas–MG. Validar antes de publicar comercialmente. Botão abre \`https://wa.me/5535999541742\` com mensagem pré-preenchida como “Olá! Gostaria de solicitar uma avaliação do meu veículo.”

## 8. Padrão técnico e entrega

- HTML semântico, CSS bem organizado e JS mínimo; herdar stack do projeto se já existir. Não adicionar backend, banco de dados ou pacote visual pesado.
- WCAG AA, contraste ≥4,5:1 para texto comum, focus ring visível, teclado funcional, alvos de toque ≥44 px, respeito a \`prefers-reduced-motion\`.
- Layout mobile-first sem scroll horizontal. Checar 375, 768, 1024 e 1440 px.
- Imagens com dimensões reservadas, carregamento lazy abaixo do Hero, mídia otimizada quando houver autorização.
- Core Web Vitals como metas de validação, não como números fictícios. Testar CTA, menu, FAQ, links e navegação por âncora.
- Entregue **A)** mapa de seções com layout desktop/mobile **B)** mini design system e estados de botões **C)** inventário imagem → copy → função **D)** copy final de cada seção **E)** componentes do esqueleto e lista de pendências.
- Antes de escrever código, faça uma checagem crítica: **o layout pareceria uma oficina premium específica chamada Car Club, ou mais um template?** Se parecer genérico, refine composição, imagem, tipografia e clareza, **sem acrescentar seções**.

**Regra final: futurismo é precisão de composição, interação e acabamento — não efeitos decorativos.** O site deve fazer a empresa parecer contemporânea e confiável, com conteúdo e prova autênticos. **Publicar no GitHub toda alteração aprovada, e só afirmar que o site está no ar após verificar a hospedagem.**
