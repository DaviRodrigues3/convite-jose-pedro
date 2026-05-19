# 🌟 Mapeamento Completo — Convite José Pedro

Roadmap de tudo que pode tornar o convite ainda mais especial.
Cada item tem **prioridade** (P0 essencial → P3 nice-to-have), **esforço** (S/M/L/XL), e **valor estimado** (⭐ a ⭐⭐⭐⭐⭐).

---

## ✅ 1. Já implementado neste release

| Item | Onde |
|---|---|
| Redesenho completo da cena (Príncipe ajoelhado com rosto, Raposa interagindo, Rosa atrás, planeta B612 redondo, vulcão, baobá, mini-asteroides) | [index.html](index.html) — bloco `.prince-scene` |
| Animações vivas: `tail-wag`, `rose-sway`, `scarf-wave` aprimorado, `crown-sparkle`, hover-reactions | [index.html](index.html) — CSS `@keyframes` |
| Citações rotativas do livro (7 frases icônicas, fade a cada 6.5s) | `.quotes-section` |
| Partículas douradas flutuantes (canvas full-screen, 22-38 partículas adaptativas) | `#dustCanvas` |
| Confete dourado ao confirmar presença (estrelas + corações + retângulos) | `triggerConfetti()` |
| Mural digital de mensagens (localStorage, cards estilo Polaroid com fita washi) | `.wishes-section` |
| Botão "Enviar para os pais" via WhatsApp | `#btnSendWish` |
| Música de fundo procedural (Web Audio API, pad ambiente C-maior com LFO, opt-in, persiste em localStorage) | `#musicBtn` |
| Efeitos sonoros (chime ao confirmar, sparkle ao tocar personagens) | `playChime()`, `playSparkle()` |
| Interatividade dos personagens (clique no Príncipe/Raposa/Rosa emite sparkles + som; rosa vibra pétalas) | `.prince-group`, `.fox-group`, `.rose-group` |
| Trilha de brilhos seguindo o cursor (desktop) | `cursor-spark` |
| Favicon (estrela dourada com céu) | [favicon.svg](favicon.svg) |
| Preview rico no WhatsApp/redes (Open Graph + Twitter Card) | [og-image.svg](og-image.svg) + meta tags |
| ARIA label no SVG da cena | `aria-label` no `<svg>` |
| Respeito ao `prefers-reduced-motion` (partículas, confete, parallax, animações pesadas desligam) | `@media (prefers-reduced-motion: reduce)` |
| Botões RSVP restaurados (Confirmar, Calendário, Compartilhar) com SVG icons | `.actions-section` |

---

## 🎨 2. Ilustração & Estética

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 2.1 | Versão dia/noite alternável da cena (modo claro vs estrelado) | P2 | M | ⭐⭐⭐ |
| 2.2 | Filtro `feTurbulence` de aquarela mais agressivo nas bordas dos paths | P3 | S | ⭐⭐ |
| 2.3 | Sombras volumétricas nos personagens (luz vinda da estrela à direita) | P2 | M | ⭐⭐⭐ |
| 2.4 | Variação sazonal: Príncipe ganha cachecol amarelo (noturno) ou vermelho (matinal) conforme hora real | P3 | M | ⭐⭐ |
| 2.5 | Modo "ilustração de capa do livro" (cores mais aquareladas, menos saturação) | P2 | M | ⭐⭐⭐ |
| 2.6 | Avião do aviador (Saint-Exupéry) caído no canto inferior do céu como easter egg estático | P3 | S | ⭐⭐ |
| 2.7 | Halo orbital ao redor do planeta (anéis em órbita) | P3 | S | ⭐⭐ |

## 🎭 3. Animações & Efeitos Visuais

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 3.1 | Cometa atravessando a tela a cada 30s (animação CSS path) | P2 | S | ⭐⭐⭐ |
| 3.2 | Satélite/nave em órbita ao planeta B612 | P3 | M | ⭐⭐ |
| 3.3 | Sol nascendo/se pondo durante o scroll (gradiente do céu muda) — referência canônica "vi 43 pores-do-sol" | P1 | M | ⭐⭐⭐⭐ |
| 3.4 | Aurora boreal sutil pulsando no horizonte do céu | P3 | M | ⭐⭐ |
| 3.5 | Estrela cadente que reage a cliques em qualquer estrela do céu | P2 | S | ⭐⭐⭐ |
| 3.6 | "Respiração" sutil no peito do Príncipe e da Raposa (scale 1.0↔1.02) | P3 | S | ⭐⭐ |
| 3.7 | Piscar dos olhos do Príncipe a cada 8-12s | P2 | S | ⭐⭐⭐ |
| 3.8 | Vulcão soltar uma baforada de fumaça a cada 20s | P3 | S | ⭐⭐ |
| 3.9 | Folha do baobá brilhar levemente ao passar mouse | P3 | S | ⭐⭐ |
| 3.10 | Páginas viram (efeito 3D "abrir o livro") na transição do intro | P2 | L | ⭐⭐⭐⭐ |

## 🔊 4. Áudio & Som

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 4.1 | Substituir pad procedural por trilha real (instrumental de "Le Petit Prince" de Hans Zimmer ou similar, royalty-free) | P1 | M | ⭐⭐⭐⭐ |
| 4.2 | Voiceover do convite (TTS browser ou gravação dos pais) | P2 | M | ⭐⭐⭐⭐ |
| 4.3 | Som de raposa ao clicar nela (yip suave) | P3 | S | ⭐⭐ |
| 4.4 | Som de vento ao passar pelo cachecol | P3 | S | ⭐⭐ |
| 4.5 | Notinha musical ao adicionar recado no mural | P2 | S | ⭐⭐⭐ |
| 4.6 | Crossfade entre trilha ambiente e chime ao confirmar | P3 | M | ⭐⭐ |

## ✨ 5. Interatividade & Easter Eggs

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 5.1 | Digitar "B612" no teclado revela uma cena oculta (avião do aviador) | P2 | M | ⭐⭐⭐⭐ |
| 5.2 | Long-press (3s) na Raposa: barra de "amizade" preenche e ela "é cativada" — sorriso muda + frase aparece | P1 | M | ⭐⭐⭐⭐⭐ |
| 5.3 | Triplo clique na Rosa: ela cora (gradient muda) + frase "Sou única em todo o universo" | P2 | S | ⭐⭐⭐ |
| 5.4 | Desenho da jiboia/elefante (Drawing #1) acessível por botão escondido no rodapé | P2 | M | ⭐⭐⭐⭐ |
| 5.5 | Caixa com a ovelha (Drawing famoso): clique e a ovelha aparece dormindo dentro | P2 | M | ⭐⭐⭐⭐ |
| 5.6 | Mini-jogo "capturar estrelas cadentes" (clique para coletar, contador no topo) | P3 | L | ⭐⭐⭐ |
| 5.7 | Tour pelos planetas do livro (Rei, Vaidoso, Bêbado, Homem de Negócios, Acendedor, Geógrafo) — modo carrossel | P3 | XL | ⭐⭐⭐⭐ |
| 5.8 | Konami code (↑↑↓↓←→←→) ativa "modo aniversariante": coroa cresce, confete contínuo, música festiva | P3 | M | ⭐⭐⭐ |

## 📝 6. Conteúdo do Evento (futuro — usuário pediu para não criar agora)

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 6.1 | Endereço da festa com mapa estilizado (planeta como pin) | P0 | M | ⭐⭐⭐⭐⭐ |
| 6.2 | Dress code visual (paleta: dourado, azul-noite, vermelho-rosa, verde-jaqueta) | P1 | S | ⭐⭐⭐⭐ |
| 6.3 | Programa da festa (cronograma com ícones estelares) | P1 | M | ⭐⭐⭐⭐ |
| 6.4 | Pix QR code para presente em dinheiro | P0 | S | ⭐⭐⭐⭐⭐ |
| 6.5 | Lista de presentes (cards com fotos clicáveis) | P1 | M | ⭐⭐⭐⭐ |
| 6.6 | Mensagem dos pais (texto em formato carta manuscrita) | P1 | S | ⭐⭐⭐⭐ |
| 6.7 | Cardápio (com ícones de comidas e bebidas servidas) | P3 | M | ⭐⭐ |
| 6.8 | Localização do estacionamento / como chegar | P2 | S | ⭐⭐⭐ |
| 6.9 | Política de presença de crianças / espaço kids | P2 | S | ⭐⭐⭐ |

## 📷 7. Memórias & Fotos

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 7.1 | Galeria mês-a-mês do 1º ano (carrossel com 12 fotos) | P0 | M | ⭐⭐⭐⭐⭐ |
| 7.2 | Timeline interativa de marcos (primeiro sorriso, primeiro dente, primeiros passos) | P1 | M | ⭐⭐⭐⭐⭐ |
| 7.3 | Foto do bebê substitui o rosto do Príncipe quando o usuário aproxima o mouse | P2 | M | ⭐⭐⭐⭐ |
| 7.4 | Mosaico de fotos enviadas pelos convidados (sobe via formulário) | P2 | XL | ⭐⭐⭐⭐ |
| 7.5 | Vídeo de 30s do bebê em loop discreto no topo | P2 | M | ⭐⭐⭐⭐ |

## ✉️ 8. RSVP & Backend

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 8.1 | RSVP real com formulário (nome, número de adultos, crianças, restrições alimentares) salvando em Google Sheets via Apps Script (grátis) | P0 | M | ⭐⭐⭐⭐⭐ |
| 8.2 | Alternativa: Firebase Firestore (dashboard em tempo real) | P1 | L | ⭐⭐⭐⭐ |
| 8.3 | Alternativa simples: Formspree ou Netlify Forms | P0 | S | ⭐⭐⭐⭐⭐ |
| 8.4 | Contador de convidados confirmados ao vivo ("32 estrelas já confirmadas") | P2 | M | ⭐⭐⭐⭐ |
| 8.5 | Lembrete automático 3 dias antes (via email/SMS para quem confirmou) | P2 | L | ⭐⭐⭐⭐ |
| 8.6 | Confirmação dupla (você confirmou + os pais receberam) com email transacional | P3 | M | ⭐⭐⭐ |
| 8.7 | Mural global de recados via Firestore (todos os convidados veem os mesmos recados) | P1 | M | ⭐⭐⭐⭐⭐ |

## 🌐 9. Compartilhamento & Social

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 9.1 | Template de Story do Instagram baixável (1080x1920) | P2 | M | ⭐⭐⭐⭐ |
| 9.2 | Filtro do Instagram com a coroa do Príncipe | P3 | XL | ⭐⭐⭐ |
| 9.3 | Card pré-renderizado para o convidado compartilhar com sua foto | P2 | M | ⭐⭐⭐ |
| 9.4 | Botão "compartilhar no WhatsApp" com mensagem pré-formatada | P1 | S | ⭐⭐⭐⭐ |
| 9.5 | Versão exportável em PDF como lembrança | P2 | M | ⭐⭐⭐⭐ |
| 9.6 | Versão para imprimir (CSS @media print) | P3 | S | ⭐⭐ |

## ♿ 10. Acessibilidade

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 10.1 | ARIA labels em cada elemento do SVG (Príncipe, Raposa, Rosa) | P0 | S | ⭐⭐⭐⭐ |
| 10.2 | `<title>` e `<desc>` dentro do SVG para leitores de tela | P1 | S | ⭐⭐⭐⭐ |
| 10.3 | Navegação completa por teclado em todos os botões | P0 | S | ⭐⭐⭐⭐⭐ |
| 10.4 | Modo alto contraste (botão alternar) | P2 | M | ⭐⭐⭐ |
| 10.5 | Tamanho de fonte ajustável (A− / A+) | P3 | M | ⭐⭐ |
| 10.6 | Anúncio dinâmico das citações por leitor de tela (`aria-live`) | P1 | S | ⭐⭐⭐⭐ |
| 10.7 | Anúncio do countdown a cada 1h ("faltam 5 dias e 12 horas") | P3 | S | ⭐⭐ |

## 🌍 11. Internacionalização

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 11.1 | Toggle PT/EN no canto superior | P2 | M | ⭐⭐⭐⭐ |
| 11.2 | Versão em Francês (tributo ao autor!) | P3 | M | ⭐⭐⭐⭐ |
| 11.3 | Espanhol para parentes hispano-falantes | P3 | M | ⭐⭐⭐ |
| 11.4 | URL params `?lang=en` | P3 | S | ⭐⭐ |

## ⚡ 12. Performance & PWA

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 12.1 | Manifest PWA (instalável no celular como app) | P1 | S | ⭐⭐⭐⭐⭐ |
| 12.2 | Service Worker para funcionar offline | P2 | M | ⭐⭐⭐⭐ |
| 12.3 | Push notification do countdown ("1 dia para a festa!") | P3 | L | ⭐⭐⭐ |
| 12.4 | Split do `index.html` em arquivos separados (CSS/JS) | P3 | M | ⭐⭐ |
| 12.5 | Lazy load dos canvases (só carrega quando visível) | P3 | S | ⭐⭐ |
| 12.6 | Pré-renderização do og-image em PNG (Puppeteer) | P2 | M | ⭐⭐⭐⭐ |
| 12.7 | Lighthouse audit ≥ 90 em todas as métricas | P2 | M | ⭐⭐⭐⭐ |
| 12.8 | Compressão dos `@font-face` base64 ou migração para `font-display: optional` | P2 | M | ⭐⭐⭐ |

## 💝 13. Personalização por convidado

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 13.1 | Link único por convidado (`?guest=Maria`) com saudação personalizada no hero | P1 | M | ⭐⭐⭐⭐⭐ |
| 13.2 | Token único de RSVP (não dá pra confirmar 2x) | P2 | M | ⭐⭐⭐⭐ |
| 13.3 | Vídeo gravado pelos pais para cada convidado VIP | P3 | XL | ⭐⭐⭐⭐ |
| 13.4 | Foto do convidado aparece como "asteroide visitante" girando no céu | P3 | L | ⭐⭐⭐⭐ |
| 13.5 | Mensagem manuscrita assinada (canvas de assinatura para deixar marca) | P3 | M | ⭐⭐⭐ |

## 🎁 14. Easter eggs do livro

| # | Item | Prio | Esforço | Valor |
|---|---|---|---|---|
| 14.1 | Desenho da jiboia engolindo o elefante (Drawing #1) — escondido | P2 | S | ⭐⭐⭐⭐⭐ |
| 14.2 | A ovelha na caixa (Drawing canônico) | P2 | S | ⭐⭐⭐⭐⭐ |
| 14.3 | Acendedor de lampião no asteroide 329 (acende/apaga a cada clique) | P3 | M | ⭐⭐⭐⭐ |
| 14.4 | A serpente amarela enrolada num canto (eg. ao final da página) | P3 | S | ⭐⭐⭐ |
| 14.5 | A rosa diz uma frase ao hover ("Pus muito esforço para ser bonita") | P2 | S | ⭐⭐⭐⭐ |
| 14.6 | Os baobás crescendo perigosamente se você esperar muito tempo na página | P3 | M | ⭐⭐⭐⭐ |
| 14.7 | Pássaros migratórios carregando o Príncipe entre seções | P3 | L | ⭐⭐⭐⭐⭐ |
| 14.8 | Quando o countdown chega a zero: chuva de estrelas + frase "Quando você olhar para o céu à noite..." | P1 | M | ⭐⭐⭐⭐⭐ |

---

## 📊 Priorização sugerida — próximos 3 sprints

### Sprint 1 (impacto alto, esforço baixo) — *"polish"*
- 6.2 Dress code visual
- 6.4 Pix QR code
- 6.6 Mensagem dos pais
- 10.1, 10.2, 10.6 Acessibilidade básica
- 12.1 PWA manifest
- 14.5 Rosa fala ao hover
- 14.8 Chuva de estrelas quando countdown zera

### Sprint 2 (conteúdo) — *"as memórias"*
- 6.1 Mapa do local
- 6.3 Programa da festa
- 7.1 Galeria mês-a-mês
- 7.2 Timeline de marcos
- 8.1 ou 8.3 RSVP real (Google Sheets ou Formspree)

### Sprint 3 (encantamento) — *"easter eggs"*
- 3.3 Sol nascendo/se pondo no scroll
- 5.2 "Cativar a raposa" (long-press)
- 5.4 Drawing #1 da jiboia
- 14.7 Pássaros migratórios entre seções
- 11.2 Versão em Francês

---

## 💭 Considerações finais

- **Manter simplicidade**: o site monolítico em arquivo único é elegante e portátil. Só split em arquivos se for adicionar dezenas de seções novas.
- **Performance > tudo**: cada animação a mais cobra um custo. Sempre testar em celular mediano.
- **Histórias > recursos**: cada item adicionado deve servir à história ("é o coração do convite, não a planilha de funcionalidades").

> _"Foi o tempo que perdeste com tua rosa que a fez tão importante."_
> — Saint-Exupéry
