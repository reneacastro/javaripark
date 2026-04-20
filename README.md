# Javari StrEat Park — Dossiê de Aquisição

Landing page confidencial para o processo de venda do Javari StrEat Park.

---

## Setup inicial (uma vez)

1. **Criar o repositório no GitHub** (privado ou público — tanto faz, como o `noindex` já evita indexação)
2. **Subir todos os arquivos** deste pacote para a raiz do repo:
   - `index.html`
   - `robots.txt`
   - `.nojekyll`
   - `README.md`
3. **Ativar GitHub Pages:**
   - `Settings` → `Pages` (menu lateral)
   - Em **Source**, escolher: `Deploy from a branch`
   - Em **Branch**, escolher `main` (ou `master`) + `/ (root)`
   - Clicar em **Save**
4. Aguardar ~1 minuto. A URL aparece no topo da página de Pages (formato `https://<user>.github.io/<repo>/`)

---

## Atualizar conteúdo

Qualquer alteração é feita direto no `index.html`:

- **Texto**: busque a seção que quer editar (estão marcadas com comentários tipo `<!-- ============== HERO ============== -->`)
- **Fotos**: trocar as URLs dos `src` das imagens (atualmente apontam para o WordPress do Javari — se mudar o site, atualizar aqui também)
- **WhatsApp / e-mail**: buscar por `5511994474544` e `oi@javaripark.com.br` para trocar se mudar o contato
- **Preço**: buscar por `990.000`

Depois de editar, commit + push. GitHub Pages atualiza em ~30 segundos.

---

## Dependências externas

A página depende de dois recursos externos:

1. **Google Fonts** (Fraunces + Manrope) — carrega automaticamente via `<link>` no `<head>`. Se o Google Fonts cair, fallback para Georgia/Arial (fallback definido no CSS)
2. **Imagens do WordPress** — todas as fotos vêm de `javaripark.com.br/wp-content/uploads/...`. Se o WP sair do ar ou as URLs mudarem, as imagens quebram. Para blindar 100%, copie as fotos para a pasta `/img/` deste repo e atualize os paths

---

## SEO / Indexação

A página está configurada para **não ser indexada** pelo Google:

- Meta tag `<meta name="robots" content="noindex, nofollow, noarchive, nosnippet">` no `<head>`
- Arquivo `robots.txt` bloqueando todos os crawlers

Só quem receber o link direto acessa. Isso é proposital: o dossiê é confidencial.

---

## Estrutura de seções

1. **Hero** — preço + CTA principal (`/investimento/` original)
2. **01 Panorama** — 8 KPIs numéricos
3. **02 A casa** — mosaico de fotos do ambiente
4. **03 Escopo da transferência** — ativos tangíveis e intangíveis
5. **Pull quote** — "Compre na sexta. Opere no sábado."
6. **04 Bus Lounge** — feature destacado
7. **05 Por que faz sentido** — 4 argumentos (cards)
8. **06 Palco e música ao vivo** — mosaico
9. **07 Parcerias** — lista de fornecedores
10. **08 Segurança jurídica e financeira** — grid de garantias
11. **09 A casa em um olhar** — galeria final + link para `/fotos`
12. **10 Próximo passo** — CTA final (WhatsApp + e-mail)

---

## Contato / autor

Dossiê interno — versão de trabalho. Para dúvidas técnicas ou ajustes, editar direto o `index.html`.
