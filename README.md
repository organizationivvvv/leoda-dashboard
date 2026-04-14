# Dashboard LEODA Players 2026

Dashboard estático de performance digital multicanal que analisa a presença digital de players do mercado.

## 📊 Métricas Analisadas

- **Instagram**: Performance de engajamento e seguidores
- **Facebook**: Seguidores e presença
- **LinkedIn**: Performance corporativa
- **YouTube**: Inscritos e visualizações
- **SEO**: Performance de otimização para motores de busca
- **PageSpeed**: Velocidade de carregamento do site
- **Google Meu Negócio (GMN)**: Avaliação e presença

## 🚀 Como Usar

### Visualizar Localmente

Basta abrir o arquivo `index.html` em qualquer navegador moderno:

```bash
# No Windows
start index.html

# No macOS
open index.html

# No Linux
xdg-open index.html
```

### Deploy no GitHub Pages

1. Crie um novo repositório no GitHub
2. Faça push dos arquivos:
   ```bash
   git init
   git add .
   git commit -m "feat: initial LEODA dashboard"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
   git push -u origin main
   ```
3. Vá em **Settings > Pages** e selecione a branch `main`
4. O GitHub Actions irá fazer o deploy automaticamente

Ou simplesmente aguarde o deploy automático via GitHub Actions (configurado para a branch `main`).

## 📁 Estrutura do Projeto

```
leoda-dashboard/
├── index.html          # Dashboard completo (HTML + CSS + JS)
├── data.json           # Dados de performance (Jan-Mar 2026)
├── chart.min.js        # Chart.js (backup local)
├── README.md           # Este arquivo
└── .github/
    └── workflows/
        └── deploy.yml  # CI/CD para GitHub Pages
```

## 🛠️ Tecnologias

- **HTML/CSS/JS vanilla** — sem build step, sem framework
- **Chart.js 4.4** via CDN
- **Google Fonts**: Poppins (títulos) + Inter (corpo)
- **GitHub Pages** para hospedagem
- **GitHub Actions** para deploy automático

## 📈 Funcionalidades

- ✅ KPIs principais com destaque visual
- ✅ Cards de tendência com delta de performance
- ✅ Posição por plataforma (Instagram, Facebook, LinkedIn, YouTube, SEO, GMN, PageSpeed)
- ✅ Filtros interativos por player
- ✅ Gráficos de barras horizontais por plataforma
- ✅ Evolução temporal de todos os players
- ✅ Rankings de touchpoints digitais e performance ponderada
- ✅ Radar multicanal (Top 5)
- ✅ Exportar CSV (todos os dados)
- ✅ Exportar PNG (cada gráfico individual)
- ✅ Seleção de mês (Jan, Fev, Mar)
- ✅ Dark mode automático (via `prefers-color-scheme`)
- ✅ Acessibilidade (skip link, ARIA labels, focus-visible)
- ✅ Loading states com skeleton spinner

## 📝 Dados

Os dados estão externalizados no arquivo `data.json` e incluem métricas de:

- **Janeiro 2026**
- **Fevereiro 2026**
- **Março 2026**

## 🎨 Customização

Para alterar cores ou adicionar novos players, edite o arquivo `data.json`:

```json
{
  "meta": {
    "players": ["Player 1", "Player 2", ...],
    "playerColors": {
      "Player 1": "#1e40af",
      "Player 2": "#9ca3af"
    }
  }
}
```

## 📄 Licença

Projeto privado — uso interno.

---

**© 2026 LEODA Players Dashboard**
