# PROMPT — Landing Page "Halloween zu zweit" (Alemanha)

> Copie tudo abaixo da linha e cole no Claude.

---

Você é um especialista em landing pages de alta conversão para infoprodutos low ticket e em copywriting nativo em alemão (Alemanha, não Áustria/Suíça). Crie uma landing page completa, responsiva e mobile-first para vender um produto digital de Halloween para casais na Alemanha.

## 1. Entregáveis técnicos

- Um único arquivo `index.html` com CSS e JS inline (sem build, pronto para deploy na Vercel).
- Fontes do Google Fonts: **"Permanent Marker"** (títulos em estilo pincel), **"Kalam"** ou **"Patrick Hand"** (textos manuscritos/destaques) e **"Nunito"** (texto corrido, para leitura fácil).
- Todo o texto visível em **alemão nativo**, natural, com tratamento informal no plural/singular ("du"/"ihr"), porque o público é de casais jovens. Nada de tradução literal do português.
- Imagens como placeholders bem marcados (`<img src="img/hero-mockup.png" alt="...">`) com comentário no HTML dizendo qual imagem colocar em cada lugar.
- Links de checkout como variáveis no topo do JS: `CHECKOUT_BASIC`, `CHECKOUT_COMPLETE`, `CHECKOUT_POPUP`.
- Mobile-first: a maioria do tráfego vem do Instagram/Facebook/TikTok no celular. Botões grandes, fonte mínima de 16px, nada de scroll horizontal.
- Página leve e rápida: imagens com `loading="lazy"` (menos a do hero), sem bibliotecas pesadas.

## 2. Identidade visual (seguir o estilo do entregável)

O entregável do produto é um pôster ilustrado chamado **"HALLOWEEN ZU ZWEIT — 9 Kostümideen für euch als Paar"**. A página tem que parecer uma extensão desse material:

- **Fundo:** papel creme/pergaminho (`#F3E9D2`) com textura sutil de papel (gradiente ou SVG noise leve).
- **Títulos de seção:** texto em **amarelo-mostarda** (`#F2B632`) dentro de uma **faixa preta com borda de pincel irregular** (brush stroke), exatamente como as etiquetas "VAMPIRE", "SKELETTE", "PIRATEN" do entregável. Faça isso com SVG/CSS (clip-path ou SVG de fundo), levemente inclinado (-1° a -2°).
- **Destaques de texto:** marca-texto amarelo pincelado atrás de palavras-chave (igual aos bullets do entregável).
- **Cores:** preto tinta `#151515`, creme `#F3E9D2`, mostarda `#F2B632`, laranja abóbora `#E8731C`, vermelho sangue `#9E1B1B` (detalhes), branco osso `#FFFDF6`.
- **Elementos decorativos desenhados à mão (SVG inline):** morcegos, teia de aranha, ossinhos, caveirinha, abóbora, estrelinhas, setas curvas desenhadas à mão ligando seções (como no pôster).
- **Bullets:** pontinho preto + texto manuscrito sobre faixa amarela.
- **Cards:** fundo branco osso, borda preta fina meio irregular, sombra deslocada (estilo "sticker"/rascunho), cantos levemente arredondados.
- **Botões CTA:** laranja abóbora com texto preto em caixa alta, borda preta grossa, sombra sólida preta deslocada (4px 4px), animação de pulso suave. No hover, a sombra diminui (efeito de "apertar").
- Clima: divertido, romântico e assustador ao mesmo tempo — **não** sombrio/terror pesado. É sobre casal se divertir junto.

## 3. Estrutura da página (nesta ordem)

### 3.1 Barra de urgência fixa no topo
Faixa preta com texto mostarda:
`🎃 Halloween ist am 31. Oktober – Angebot endet in: [contador]`

**Importante:** o contador deve contar até a data real **31.10.2026 23:59 (horário de Berlim)**, não um contador falso que reinicia. Na Alemanha, contador falso é prática desleal (UWG) e pode gerar problema. A urgência real do Halloween já é forte o suficiente.

### 3.2 Hero
- Rótulo pequeno: `HALLOWEEN ZU ZWEIT • KOSTÜMGUIDE FÜR PAARE`
- Headline (H1): **"180+ Pärchen-Kostüme für Halloween – Schnell zusammengestellt, garantiert ein Hingucker"**
- Subheadline: "Schluss mit Last-Minute-Stress: Wählt euer Motto, stellt das Outfit mit Sachen zusammen, die ihr großteils schon habt, und werdet das Paar, über das auf der Party alle reden."
- Mockup do material (placeholder: tablet + celular mostrando as páginas do guia).
- CTA: `JA, ICH WILL DEN GUIDE!` → rola até a seção de planos.
- Selo abaixo: `🔒 100 % sichere Zahlung • ⚡ Sofortiger Zugang per E-Mail`

### 3.3 "FÜR WEN IST DAS?" (público-alvo) — 4 cards com ícone desenhado
- **Paare, die zusammen auf eine Party gehen** – "Ihr wollt als Team auffallen, nicht als zwei Einzelkostüme."
- **Last-Minute-Planer** – "Halloween ist in ein paar Tagen und ihr habt noch keine Idee?"
- **Paare mit kleinem Budget** – "Viele Looks klappen mit Kleidung aus dem eigenen Schrank."
- **Fotofans & Social-Media-Paare** – "Kostüme, die auf Fotos und in Reels richtig wirken."

### 3.4 "WAS IHR BEKOMMT" (benefícios) — 5 bullets com faixa amarela
- **180+ illustrierte Kostümideen für Paare** – von klassisch bis kreativ
- **Fertige Outfit-Listen** – genau was ihr braucht, Teil für Teil
- **Make-up- und Detail-Tipps** – damit der Look komplett wirkt
- **Nach Stil sortiert** – gruselig, romantisch, lustig, Kult-Paare
- **Sofort umsetzbar** – auch mit Kleidung, die ihr schon zu Hause habt

### 3.5 "SO SIEHT ES INNEN AUS" (prévia)
- Carrossel horizontal infinito das páginas internas (placeholders `img/seite-01.png` …). Pausa no hover/toque, clique abre lightbox ampliada.
- Inclua como primeira página o pôster "9 Kostümideen für euch als Paar" (Vampire, Skelette, Piraten, Engel und Teufel, Spinnen-Paar, Hexe und Hexer, Harley und Joker, Wildwest, Mumien).
- Texto abaixo: `Tippe auf eine Seite, um sie größer zu sehen.`

### 3.6 "EXKLUSIVE BONI" — 4 cards com mockup + "Wert: X €" riscado
- **Bonus 01: Halloween-Make-up Schritt für Schritt** – Einfache Anleitungen für Skelett, Vampir, Joker & Co. (Wert: 9 €)
- **Bonus 02: 30 Last-Minute-Kostüme in unter 1 Stunde** – Für alle, die wirklich spät dran sind. (Wert: 7 €)
- **Bonus 03: Pärchen-Fotoposen für Halloween** – Damit eure Fotos genauso gut aussehen wie eure Kostüme. (Wert: 7 €)
- **Bonus 04: Halloween-Party-Checkliste** – Deko, Snacks, Drinks und Playlist für den perfekten Abend. (Wert: 5 €)

### 3.7 Resumo de valor (ancoragem)
Card estilo "nota fiscal rabiscada":
- Kostümguide "Halloween zu zweit": 27 €
- 4 exklusive Boni: 28 €
- **Gesamtwert: 55 €**
- **Heute nur: 17 €** (com marca-texto amarelo e o "55 €" riscado em vermelho)

### 3.8 "WÄHLT EUER PAKET" (planos) — 2 cards lado a lado (empilhados no mobile, **plano Completo em cima no mobile**)
Contador repetido acima: `Angebot gilt nur bis Halloween – endet in: [dd Tage : hh Std : mm Min : ss Sek]`

**Card 1 – Basis-Paket — 10 €** (einmalige Zahlung)
- ✅ Kostümguide "Halloween zu zweit"
- ✅ Lebenslanger Zugang
- ❌ Ohne Make-up-Anleitung
- ❌ Ohne Last-Minute-Kostüme
- ❌ Ohne Fotoposen
- ❌ Ohne Party-Checkliste
- Botão (estilo secundário, contorno): `Basis-Paket wählen` → **NÃO vai para o checkout; abre o pop-up (3.12)**

**Card 2 – Komplett-Paket — 17 €** (einmalige Zahlung) — selo "BELIEBTESTE WAHL 🎃", borda laranja, levemente maior
- ✅ Kostümguide "Halloween zu zweit"
- ✅ Lebenslanger Zugang
- ✅ Alle 4 exklusiven Boni
- ✅ Zukünftige Updates kostenlos
- Linha: `Gesamtwert: ~~55 €~~ → heute nur 17 €`
- Botão (CTA principal): `JA, ICH WILL DAS KOMPLETT-PAKET` → `CHECKOUT_COMPLETE`

Abaixo de ambos: `🔒 Sichere Zahlung • Alle Preise inkl. MwSt.`

### 3.9 "DAS SAGEN ANDERE PAARE" (depoimentos)
Carrossel de prints de depoimentos (placeholders `img/feedback-01.png`…). **Não invente depoimentos**: deixe só os espaços para as imagens reais com comentário `<!-- substituir por depoimentos reais -->`.

### 3.10 "7 TAGE GARANTIE"
Selo desenhado à mão + texto:
"Wenn euch der Guide innerhalb von 7 Tagen nicht gefällt, schreibt uns einfach eine E-Mail – ihr bekommt 100 % eures Geldes zurück. Ohne Fragen, ohne Stress."

### 3.11 "HÄUFIGE FRAGEN" (FAQ em acordeão)
1. **Wie bekomme ich den Guide?** – Direkt nach der Zahlung per E-Mail als PDF – auf Handy, Tablet oder PC nutzbar.
2. **Brauche ich teure Kostüme aus dem Shop?** – Nein. Viele Ideen lassen sich mit Kleidung umsetzen, die ihr schon habt, plus ein paar günstige Details.
3. **Ist das auch etwas für Last-Minute?** – Ja! Mit dem Bonus "30 Last-Minute-Kostüme" schafft ihr es sogar am Abend selbst.
4. **Funktioniert das auch für gleichgeschlechtliche Paare oder Freunde?** – Natürlich. Die Ideen passen für jedes Duo.
5. **Wie funktioniert die Garantie?** – 7 Tage lang, eine E-Mail genügt, ihr bekommt euer Geld vollständig zurück.

CTA final: `JETZT PAKET WÄHLEN` → rola até os planos.

### 3.12 Pop-up (downsell ao clicar no Basis-Paket)
Abre ao clicar em "Basis-Paket wählen", com overlay escuro e animação de entrada (bounce leve). Visual: card creme com faixa preta-mostarda no topo.
- Faixa: `⚡ EINMALIGES ANGEBOT!`
- Título: **"Warte! Hol dir doch alles – mit Rabatt."**
- Texto: "Für nur ein paar Euro mehr bekommst du das Komplett-Paket mit allen 4 Boni."
- Preço: `Statt ~~17 €~~ nur [PREÇO_POPUP] €`
- ✅ Kompletter Kostümguide ✅ Alle 4 Boni inklusive ✅ Lebenslanger Zugang
- Botão principal: `JA, KOMPLETT-PAKET FÜR [PREÇO_POPUP] €` → `CHECKOUT_POPUP`
- Link pequeno embaixo: `Nein danke, ich bleibe beim Basis-Paket für 10 €` → `CHECKOUT_BASIC`
- Botão "×" para fechar (fecha e volta à página, sem redirecionar).

### 3.13 Rodapé
- `© 2026 Halloween zu zweit. Alle Rechte vorbehalten.`
- Links obrigatórios na Alemanha: **Impressum**, **Datenschutzerklärung**, **AGB**, **Widerrufsbelehrung** (como `href="#"` com comentário para eu preencher).
- Aviso: "Dies ist ein digitales Produkt. Es wird kein physischer Artikel versendet."

## 4. Comportamentos em JavaScript
- Contador regressivo real até 31.10.2026 23:59 (Europe/Berlin), atualizando a barra do topo e o dos planos. Depois da data, mostrar "Angebot beendet".
- Todos os CTAs com scroll suave até `#pakete`.
- Pop-up de downsell disparado só pelo botão do Basis-Paket; fecha com ×, clique no overlay ou tecla Esc.
- Carrossel infinito com pausa no hover/toque e lightbox.
- FAQ em acordeão (um aberto por vez).
- Animação de "fade-up" suave nas seções ao rolar (IntersectionObserver), respeitando `prefers-reduced-motion`.
- Repassar os parâmetros UTM da URL para os links de checkout (para rastreamento de anúncios).

## 5. Regras de copy
- Alemão natural, curto e direto; frases de no máximo ~20 palavras.
- Preços sempre no formato alemão: `17 €`, `13,90 €` (vírgula decimal, € depois do número).
- Sem promessas exageradas; tom leve, divertido, um pouco de humor de casal.
- Repetir o CTA pelo menos 4 vezes ao longo da página.

Me entregue o código completo do `index.html`, sem cortar nenhuma parte.
