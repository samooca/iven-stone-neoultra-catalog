# 🎨 ComfyUI Workflows - Iven Stone Nuovolam Catalog

Repositório de workflows do ComfyUI utilizados para geração e edição de imagens do catálogo da linha **Nuovolam** (Iven Stone).

## 📋 Visão Geral

Esta pasta contém os workflows JSON otimizados para criação de imagens de alta qualidade para o catálogo, focando em:

- **Ambientações de luxo** para showcase dos produtos
- **Consistência visual** dos materiais reais da linha Nuovolam
- **Qualidade editorial** compatível com revistas de arquitetura e design de interiores

## 🎯 Modelos Principais

### Flux (Recomendado)
- **Modelo base**: Flux.1 Dev / Flux.2 Dev
- **Uso**: Geração de ambientações e cenários de luxo
- **Justificativa**: Melhor equilíbrio entre qualidade fotográfica, controle de composição e fidelidade a prompts detalhados

### Modelos Complementares
- **QwenImage Edit**: Edição e refinamento de imagens existentes
- **ImageZ Turbo**: Geração rápida para prototipagem
- **HunyuanImage**: Alternativa para variações específicas

## 🔧 Workflows Disponíveis

### 1. `ambientacao-base.json`
**Propósito**: Geração de ambientes de luxo (cozinhas, salas, banheiros) com iluminação natural e composição editorial.

**Nodes principais**:
- Flux Checkpoint Loader
- CLIP Text Encode (Prompt + Negative)
- KSampler (Configurações otimizadas para qualidade)
- VAE Decode
- Save Image

**Configurações recomendadas**:
- Steps: 30-50
- CFG Scale: 7.0-9.0
- Sampler: euler_ancestral ou dpm++_2m
- Scheduler: normal
- Resolution: 1024x1024 ou 1216x832 (landscape)

---

### 2. `material-consistency-ipadapter.json`
**Propósito**: Aplicar materiais reais da linha Nuovolam (mármores, granitos, superfícies ultracompactas) em ambientes gerados, mantendo fidelidade às texturas e veios.

**Tecnologias utilizadas**:
- **IP Adapter** (principal): Para transferência de estilo e textura dos materiais
- **Redux**: Alternativa para controle mais fino de características
- **Tile ControlNet**: Para preservação de detalhes em alta resolução

**Fluxo de trabalho**:
1. Carregar imagem de referência do material real (ex: Calacatta Gold, Nero Marquina)
2. Gerar ambiente base com Flux
3. Aplicar IP Adapter com peso 0.7-0.85 para integração natural
4. Ajustar iluminação e sombras para coerência

**Materiais de referência**:
- **Solid Colors**: Absolute White, Concrete Grey, Cream, Pure White Matte
- **Marble Series**: Calacatta White, Statuario Venato, Nero Marquina, Armani Dark Grey

---

### 3. `bookmatch-generation.json`
**Propósito**: Criar composições bookmatch perfeitas para a linha Marble Series, onde os veios dos mármores se conectam de forma seamless.

**Características especiais**:
- Geração de pares espelhados de imagens
- Controle preciso de simetria
- Preservação da continuidade dos veios

**Produtos aplicáveis**:
- Calacatta Gold
- Statuario White
- Bianco Venato
- Taj Mahal Pearl
- Todos os materiais da Marble Series

---

### 4. `upscale-finalization.json`
**Propósito**: Upscale de imagens para qualidade de impressão editorial (300 DPI mínimo).

**Pipeline**:
1. Imagem base (1024x1024 ou similar)
2. Upscale 2x ou 4x com modelo especializado
3. Refinamento de detalhes com ControlNet Tile
4. Correção de artefatos e sharpening sutil

**Modelos de upscale recomendados**:
- 4x-UltraSharp
- RealESRGAN_x4plus
- SwinIR_4x

**Output final**: 4096x4096 ou superior para impressão de alta qualidade

---

### 5. `product-showcase.json`
**Propósito**: Geração de imagens de produto isolado com fundo neutro ou ambientação minimalista para páginas de especificações técnicas.

**Características**:
- Iluminação de estúdio controlada
- Fundo neutro (branco, cinza, preto) ou ambiente minimalista
- Foco em texturas e acabamentos (Matte, Polished, Soft, Brushed, Leather, Textured)

---

### 6. `inpaint-outpaint.json`
**Propósito**: Edição cirúrgica de imagens existentes (extensão de canvas, correção de áreas específicas, adição de elementos).

**Casos de uso**:
- Expandir ambiente para formato de página dupla
- Corrigir inconsistências em materiais
- Adicionar elementos decorativos (vasos, plantas, objetos)
- Remover elementos indesejados

## 📁 Estrutura de Arquivos
