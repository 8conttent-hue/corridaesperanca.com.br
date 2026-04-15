# CLAUDE.md — CORRIDAESPERANCA

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** CORRIDAESPERANCA
**Nicho:** Esportes e Fitness
**Keywords:** Ola Me chamo Rodolfo Esperanca aqui e o cantinho que uso com
**Paleta de cores:** forest | **Fonte:** outfit

Olá! Me chamo Rodolfo Esperança, aqui é o cantinho que uso com minha esposa para dividir nossa vasta experiência com corridas de rua. Sejam muito bem vindos ao meu espaço. Sou corredor profissional a mais de 10 anos e decidi junto a minha esposa, Marcia Rodrigues , a criar o corrida esperança. Oi! Muito prazer, Sou a Marcia Esperança, co-fundadora do Corrida esperança, corredora profissional a mais de 8 anos e esposa do Rodrigo. Junto ao meu marido, demos inicio a este belo projeto, compartilhamos todos os nossos conhecimentos adquiridos ao longo dos anos nas ruas desse Brasil. Tivemos a ideia de criar esse blog na intenção de ajudar pessoas que estão se interessando por corrida ou corredores já experientes, pois quando começamos nesse mundo não tinha muito conteúdo na internet.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-C |
| Hero | Hero-C |
| Features | Features-J |
| About Section | About-J |
| Posts | Posts-B |
| Footer | Footer-A |
| Página Sobre | Sobre-A |
| Página Contato | Contato-D |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
