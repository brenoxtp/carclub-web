# PROMPT — ESQUELETO DE LANDING PAGE | CAR CLUB CENTRO AUTOMOTIVO

## Papel e objetivo
Atue como Engenheiro Front-End Sênior, Diretor de Arte e Especialista em CRO. Crie o **esqueleto estrutural e visual (desktop + mobile)** de uma landing page premium para a Car Club Centro Automotivo, em Três Pontas/MG. O objetivo comercial é transformar visitantes em conversas qualificadas de orçamento pelo WhatsApp.

**Importante:** construa somente o esqueleto e seus componentes reais. Não invente backend, painel, catálogo, formulário de lead ou páginas adicionais. Não transforme a página em um template genérico de mecânica.

## Referências obrigatórias
- Ficha da empresa e galeria: https://www.google.com/maps/place/Car+Club+Centro+Automotivo/
- Site institucional: https://www.oficinacarclubtp.com.br/
- Identidade de marca: https://leonebrands.com.br/portfolio/carclub-centro-automotivo/
- Instagram: https://www.instagram.com/oficinacarclub/
- Metodologia de design: https://github.com/nextlevelbuilder/ui-ux-pro-max-skill

## Aplique a skill UI UX Pro Max antes de decidir o layout
1. Se estiver instalada no projeto, leia `.claude/skills/ui-ux-pro-max/SKILL.md` e `references/quick-reference.md`. Caso não esteja, consulte o repositório oficial e instale-a pelo procedimento documentado antes de usar seus scripts. Não afirme que executou comandos que não executou.
2. Com Python disponível, gere o design system a partir da ferramenta da skill:
   `python .claude/skills/ui-ux-pro-max/scripts/search.py "premium automotive bodywork painting local service conversion" --design-system -p "Car Club Centro Automotivo"`
3. Complemente as decisões com as buscas `--domain landing` (hero, prova visual e CTA), `--domain ux` (contraste, responsividade e navegação) e `--stack html-tailwind` apenas se esse stack for adotado.
4. Respeite a **identidade preexistente da Car Club** acima de recomendações estéticas genéricas. Consulte e justifique o padrão escolhido; documente tokens, tipografia, espaçamento, componentes e comportamento mobile.

## Identidade e linguagem
- Conservar logotipo, preto/grafite, laranja da marca e o universo visual de funilaria e pintura premium.
- Tipografia forte, bem legível; contrastes consistentes; espaços generosos; fotos reais com protagonismo.
- Visual sofisticado e técnico sem neon, degradês decorativos, cards idênticos em excesso, textos gigantes ou animações sem função.
- Copy direta, brasileira, segura e humana. Proposta sugerida: **"Seu carro merece atenção em cada detalhe."**
- Falar principalmente de pintura, funilaria, polimento/estética e reparos de seguradora, conforme fontes oficiais. Não criar promessas, números, avaliações, garantias ou prazos sem evidência.

## Protocolo para imagens (OBRIGATÓRIO)
Antes de posicionar qualquer foto, ABRA cada imagem e registre o que ela de fato mostra. Priorize a galeria do Google Maps e o site oficial. Não deduza conteúdo apenas pelo nome do arquivo ou URL. Confira permissão de reutilização e peça autorização quando necessário.

Imagens oficiais complementares para verificar:
- Logotipo: https://d4polyhz8pjtz.cloudfront.net/6269/cor1logo21-20240722130726.png
- Imagem promocional oficial: https://d4polyhz8pjtz.cloudfront.net/6269/paraquemvalorizacadadetalhedoseucarro-20240723150220.png
- Polimento (ilustração do site oficial): https://d4polyhz8pjtz.cloudfront.net/6269/quero-saber-mais-20240716155658_400.png
- Acabamento (ilustração do site oficial): https://d4polyhz8pjtz.cloudfront.net/6269/quero-saber-mais-20240716155734_400.png
- Colisão (ilustração do site oficial): https://d4polyhz8pjtz.cloudfront.net/6269/quero-saber-mais-20240716155626_400.png

**Regra visual:** fachada real = identidade e localização; profissional realmente trabalhando = competência; foto real de serviço = benefício concreto; veículo comprovadamente finalizado = evidência de resultado. Imagens ilustrativas não são portfólio, e o banner promocional não é prova de equipe real. Se faltar foto com direito de uso, deixe um slot claramente identificado para substituição, nunca invente resultados, profissionais ou antes/depois.

## Estrutura exata — mesma ordem no mobile
### 1. Header
Logotipo oficial à esquerda, links âncora "Serviços", "Trabalhos", "Sobre", "Localização" e botão laranja "Solicitar orçamento". No mobile, menu acessível, compacto e CTA fácil de acessar.

### 2. Hero — oferta compreendida imediatamente
Headline: "Seu carro merece atenção em cada detalhe."
Subheadline curta: serviços de funilaria, pintura e estética em Três Pontas, com foco em qualidade de acabamento e atendimento cuidadoso.
CTA principal: "Solicitar orçamento pelo WhatsApp".
**Imagem:** foto real mais forte da oficina, fachada, instalações ou carro efetivamente atendido; escolher só depois de inspeção. Desktop: texto e imagem em composição editorial com hierarquia nítida. Mobile: texto, CTA visível e imagem otimizada na sequência. Evite sobrepor texto em áreas de foto sem contraste.

### 3. Serviços — clareza de solução
Quatro blocos: **Pintura automotiva**, **Funilaria**, **Polimento e estética**, **Reparos de seguradora**. Cada um deve ter título, descrição curta, imagem condizente e CTA contextual.
**Imagens:** uma foto correspondente a cada serviço; usar imagens oficiais ilustrativas apenas com identificação adequada. Não usar o mesmo veículo aleatoriamente em todos os cards.

### 4. Trabalhos realizados — provar antes de prometer
Galeria responsiva com veículos ou detalhes de acabamento comprovadamente realizados pela Car Club.
**Imagens:** escolher exclusivamente registros reais e identificáveis da oficina. Dar destaque a fotos de acabamento, não a imagens genéricas. Comparação antes/depois só quando houver fotos do mesmo carro, autorizadas e verificadas. Quando não houver prova, criar a estrutura vazia com indicação de materiais necessários.

### 5. Diferenciais — por que confiar
Composição assimétrica: fotografia real da estrutura/equipamentos/profissional + três a quatro benefícios específicos verificados, por exemplo atenção aos detalhes, transparência, qualidade de acabamento e atendimento.
Evitar números artificiais, medalhas e superlativos não comprovados.

### 6. Sobre a Car Club — credibilidade humana
Bloco editorial com breve apresentação institucional e visão da empresa.
**Imagem:** fachada, oficina ou equipe real e autorizada; não usar foto de banco de imagens como se fosse da equipe.
CTA secundário: "Conhecer nossa oficina" apontando para localização.

### 7. Avaliações reais + FAQ — reduzir objeções
Se houver autorização e conteúdo verificável, apresentar avaliações reais do Google com atribuição e link à fonte. Nunca criar comentários ou estrelas.
FAQ com quatro objeções úteis: como solicitar avaliação/orçamento; quais serviços; seguradoras; como funciona o atendimento. Respostas devem ser verificadas.

### 8. Localização + CTA final + Footer
Mapa incorporado (ou link estável de rotas), endereço **Rua José Carlos Andrade, 205, Três Pontas–MG**, condicionado à checagem final.
Contato/WhatsApp previamente divulgado: **(35) 99954-1742**, validar antes de publicar. CTA final "Falar com a Car Club".
Footer com logo, endereço, redes e links úteis.

## Comportamento e critérios de conversão
- Caminho psicológico: entender o serviço → ver provas → confiar → entrar em contato.
- Botão fixo de WhatsApp no mobile com espaço seguro e sem cobrir conteúdo.
- CTAs com ação real e mensagem pré-preenchida contextualizada.
- Mobile-first, HTML semântico, headings corretos, contraste WCAG AA, foco visível, controles tocáveis (~44px), estados claros, sem rolagem horizontal.
- Imagens com tamanho reservado, alt descritivo, otimização WebP/AVIF e lazy load fora do Hero.
- Não usar números de avaliação, prazos, garantias, "9 anos", fotos de clientes, parceiros ou marcas de seguradoras sem conferência.

## Saída esperada
Entregar **(A)** tabela de inventário de imagens: URL/origem, conteúdo visual confirmado, função psicológica, seção e estado da licença; **(B)** esqueleto da landing page com a hierarquia acima, mostrando layout mobile e desktop, tipo de imagem, texto e CTA de cada seção; **(C)** mini design system da Car Club: cores validadas, tipografia, grids, espaçamento, responsividade e botões; **(D)** componentes básicos necessários para futura implementação.

Não inventar novas seções ou alterar a ordem. Não implementar recursos complexos nem publicar uma versão comercial antes da validação dos materiais. Se houver acesso ao projeto e solicitação de desenvolvimento, implementar o esqueleto com os arquivos existentes, sem reescrever identidade e conteúdo factual.
