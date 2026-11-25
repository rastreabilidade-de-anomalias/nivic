# NIVIC — Núcleo de Investigação e Verificação de Informação Científica

Protótipo inicial de um chatbot para combater a desinformação científica, verificar informações e explicar pesquisas em linguagem simples.

> **Versão de demonstração:** todas as respostas são **simuladas** (pré-escritas) e aparecem com a etiqueta "Simulação". Nenhuma análise real é feita nesta versão.

## Funcionalidades

- Página inicial com logotipo, descrição e o campo "O que vamos investigar hoje?"
- Chat com envio e recebimento de mensagens
- Classificação das afirmações: **Confirmada**, **Falsa**, **Enganosa**, **Inconclusiva** e **Não verificada**, cada uma com explicação e justificativa
- Modo **Pesquisa em PDF**: resumo (objetivo, método, resultados, limitações) e glossário de termos técnicos
- Modo **Vídeo ou link**: análise de afirmações com a minutagem dos trechos
- Opção de anexar documento ou imagem
- Botão de microfone (demonstração)
- Histórico de conversas (salvo no navegador) e botão "Nova análise"
- Layout adaptado para celular e computador

### Exemplos com resposta pronta

| Tema | Classificação |
|---|---|
| Alimento que "cura" doença | Enganosa |
| Vacinas causam autismo | Falsa |
| Antenas 5G espalham o coronavírus | Falsa |
| Aquecimento global causado pelo ser humano | Confirmada |
| Chocolate amargo melhora a memória | Inconclusiva |
| Qualquer outra pergunta | Não verificada |

## Como rodar no computador

Basta abrir o arquivo `index.html` no navegador. Não precisa instalar nada.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (ex.: `nivic`).
2. Envie os arquivos desta pasta (`index.html`, `README.md`, `LICENSE`, `.nojekyll`, `.gitignore`).
   - Pelo site: **Add file → Upload files** e arraste os arquivos.
   - Ou pelo terminal:
     ```bash
     git init
     git add .
     git commit -m "Primeira versão do NIVIC"
     git branch -M main
     git remote add origin https://github.com/SEU-USUARIO/nivic.git
     git push -u origin main
     ```
3. No repositório, vá em **Settings → Pages**.
4. Em **Source**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)` e clique em **Save**.
5. Em 1 ou 2 minutos o app estará em `https://SEU-USUARIO.github.io/nivic/`.

> Os arquivos `.gitignore` e `.nojekyll` começam com ponto e podem ficar ocultos no seu computador. Eles são opcionais: o app funciona só com o `index.html`.

## Estrutura

```
index.html   → o app completo (HTML, CSS e JavaScript em um único arquivo)
README.md    → este arquivo
LICENSE      → licença MIT
.nojekyll    → faz o GitHub Pages servir os arquivos sem processamento
.gitignore   → arquivos ignorados pelo Git
```

## Próximos passos

- Integração com inteligência artificial para análises reais
- Consulta a bases científicas (PubMed, SciELO, Cochrane)
- Leitura real de PDFs e transcrição de vídeos

## Aviso

Protótipo acadêmico. As respostas não representam análise médica ou científica real e não substituem a orientação de profissionais.
