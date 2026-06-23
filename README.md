# Iven Stone | Catálogo Neo Ultra ✨

> **Transformando superfícies em experiências arquitetônicas de alto luxo**

---

## 🎯 Visão Geral do Projeto

O Catálogo Neo Ultra é uma publicação editorial de luxo que posiciona a Iven Stone como referência absoluta em superfícies ultracompactas de alto padrão. Mais do que um mostruário de produtos, é uma **ferramenta estratégica de vendas** integrada ao showroom de 5.000m², projetada para seduzir arquitetos, influenciar marmoristas e validar escolhas junto aos clientes finais.

### Conceito Central
**"A Moldura Invisível"** — O design desaparece para que a pedra seja a única protagonista. Minimalismo, respiro visual e ritmo editorial inspirados em publicações como *Architectural Digest* e *Wallpaper**.

---

## 👥 Personas Estratégicas

O catálogo foi desenvolvido para dialogar com três perfis distintos da cadeia de especificação:

### 1. O Arquiteto Visionário (Especificador)
- **Busca:** Exclusividade geológica, narrativa sensorial, autoria
- **Linguagem:** "Expressão do espaço", "Legado atemporal", "Fusão entre arte e ciência"
- **Como seduzir:** Storytelling poético, ambientes de luxo, referências de revistas

### 2. O Marmorista Parceiro (Influenciador-Chave)
- **Busca:** Processabilidade, margem, suporte técnico, logística
- **Linguagem:** "Alto rendimento", "Precisão técnica", "Sem limitações"
- **Como seduzir:** Fichas técnicas claras, qualidade da chapa, confiabilidade

### 3. O Cliente Final de Alto Padrão (Validador)
- **Busca:** Status, exclusividade, valorização patrimonial, bem-estar
- **Linguagem:** "Exclusividade", "Valor atemporal", "Sofisticação"
- **Como seduzir:** Ambientes decorados, prova social, experiência no showroom

---

## 📐 Estrutura Editorial

O catálogo segue um **ritmo de revista de arquitetura** com máximo de 4 produtos por página:

### Páginas 01-04: A Sedução (Front of Book)
- Manifesto da marca
- Arquiteturas impactantes
- Textos poético-sensoriais

### Páginas 05-14: Coleção Solid Colors
- Superfícies uniformes e minimalistas (17 produtos)
- Grids de 4 produtos + páginas de destaque dramático
- Foco em durabilidade e resistência climática

### Páginas 15-24: Coleção Marble Series
- Mármores ultracompactos com veios únicos (15 produtos)
- **Tecnologia Bookmatch** (padrão seamless)
- Entrevistas com arquitetos e ensaios abstratos

### Páginas 25-32: Apêndice Técnico Premium (Back of Book)
- Curadoria e manutenção
- Arte da instalação
- Garantias e certificações
- Tabelas técnicas completas

**Total estimado:** 32-40 páginas (múltiplo de 4 para impressão offset)

---

## 🎨 Identidade Visual

### Paleta de Cores
- **Fundo:** Alabastro `#F7F5F0` (off-white quente, papel de algodão)
- **Texto:** Obsidiana `#1A1A1A` (cinza profundo, não preto puro)
- **Acento:** Bronze Envelhecido `#A89F91` (detalhes sutis)

### Sistema Tipográfico
- **Títulos/Manifesto:** Cormorant Garamond (serifada elegante, alto contraste)
- **Nomes das Pedras:** Cinzel (CAIXA ALTA, letter-spacing 0.15em)
- **Corpo/Técnico:** Inter (sans-serif geométrica, invisível)

### Regras de Layout
- **Espaço negativo:** Mínimo 40% da página deve "respirar"
- **Grid:** Assimétrico de 12 colunas
- **Alinhamento:** Texto sempre à esquerda (ragged right), nunca justificado
- **Bleed crossover:** Imagens que vazam 20-30% da próxima página

---

## 📦 Estrutura do Repositório
iven-stone-neoultra-catalog/
├── README.md # Este arquivo (visão geral do projeto)
├── .gitignore # Arquivos ignorados pelo Git
├── produtos.xlsx # Catálogo completo de produtos
│
├── docs/ # Documentação estratégica
│ ├── brand-guidelines.md # Diretrizes de marca e tom de voz
│ ├── personas.md # Perfis de público-alvo
│ ├── editorial-template.md # Template de layout e ritmo editorial
│ ├── product-catalog.md # Catálogo técnico de produtos
│ ├── reference-excerpts.md # Trechos de catálogos de referência
│ └── showroom-integration.md # Estratégia de integração catálogo-showroom
│
├── content/ # Conteúdo textual
│ ├── manifesto.md # Texto da página de abertura
│ ├── solid-colors-copy.md # Copy da coleção Solid Colors
│ ├── marble-series-copy.md # Copy da coleção Marble Series
│ └── tech-appendix.md # Apêndice técnico
│
├── assets/ # Ativos visuais
│ ├── logos/ # Logotipos Iven Stone e Neo Ultra
│ ├── products/ # Fotos das lâminas (texturas)
│ ├── environments/ # Fotos de ambientes decorados
│ └── fonts/ # Fontes (Cormorant, Cinzel, Inter)
│
└── comfyui/ # Workflows de geração de imagens
├── workflows/ # JSONs dos fluxos ComfyUI
├── prompts/ # Banco de prompts otimizados
└── docs/ # Documentação técnica

---

## 🛠 Tech Stack de Produção

### Edição e Versionamento
- **Git + GitHub Desktop:** Controle de versão e colaboração
- **VS Code:** Editor de texto com suporte a Markdown e tabelas
- **Obsidian:** Gestão de conhecimento e brainstorm

### Geração Visual
- **ComfyUI (Flux2 Dev FP8):** Geração de ambientes de luxo
- **QwenImage Edit:** Edição e refino de imagens
- **ImageZ Turbo:** Upscale de alta qualidade
- **Wan2.2 / LTX2:** Geração de vídeos promocionais
- **QwenVL:** Análise e extração de detalhes de imagens

### Configurações Recomendadas (Flux2 Dev)
- **Sampler:** Euler
- **Steps:** 20-25
- **CFG Scale:** 2.5-3.5
- **Scheduler:** Simple ou Beta
- **IP Adapter Redux:** Weight 0.5-0.7 para injeção de texturas reais

---

##  Integração com Showroom

O catálogo é parte de um **ecossistema phygital** (físico + digital) de 5.000m²:

### Jornada do Visitante
1. **Chegada:** Ambientes simulados (cozinha, sala, lavabo) com materiais reais
2. **Descoberta:** Catálogo físico presente nas bancadas como "convite silencioso"
3. **Expansão:** QR Codes em cada ambiente levam ao catálogo digital com zoom 400%
4. **Fechamento:** Catálogo entregue como "lembrança de luxo" pós-visita

### Eventos Semanais
- Chefs convidados (cozinha italiana, japonesa, etc.)
- Uso das bancadas Neo Ultra como palco gastronômico
- Conexão entre experiência sensorial (sabores) e tátil (pedras)

---

## 📝 Diretrizes de Conteúdo

### Tom de Voz
- **Arquétipo:** O Criador / O Governante
- **Somos:** Exclusivos, Técnicos, Atemporais, Sensoriais
- **Não somos:** Populares, Baratos, Trendy, Industriais

### Palavras de Poder ✅
"Majestade", "Tátil", "Geologia", "Arquitetura", "Legado", "Escultural", "Expressão", "Fusão", "Permanece", "Atemporal", "Cristalização", "Profundidade"

### Palavras Proibidas 🚫
"Barato", "Promoção", "Oferta", "Legal", "Bonito", "Custo-benefício", "Resistente" (use "Durabilidade estética")

---

## 🚀 Como Contribuir

### Fluxo de Trabalho
1. **Edite localmente** no VS Code ou Obsidian
2. **Teste o Markdown** com `Ctrl+Shift+V` (preview)
3. **Commit semântico:** `feat: add product descriptions`, `docs: update personas`
4. **Push via GitHub Desktop**

### Convenções
- **Arquivos .md:** Use GitHub Flavored Markdown (GFM)
- **Tabelas:** Máximo 4 colunas para legibilidade
- **Imagens:** Salve em `assets/` com nomes descritivos (ex: `calacatta-gold-texture.jpg`)
- **Prompts:** Sempre em inglês para melhor resultado nos modelos de IA

---

## 📊 Métricas de Sucesso

- Taxa de conversão de visita ao showroom → especificação
- Uso do catálogo pelo marmorista como argumento de venda
- Tempo médio de permanência do arquiteto no showroom
- Scan de QR Codes e interação com versão digital

---

## 📞 Contato e Recursos

- **Showroom Iven Stone:** [Endereço completo]
- **Site:** [URL do site]
- **Redes Sociais:** @ivenstone (Instagram, LinkedIn)

**Última atualização:** Junho 2026  
**Versão do documento:** 2.0

---

*"A verdadeira profundidade só pode ser sentida ao vivo."*
