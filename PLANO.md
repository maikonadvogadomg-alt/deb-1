# PLANO DO PROJETO: HTML/CSS/JS

> Gerado automaticamente pelo SK Code Editor em 14/05/2026, 14:51:10
> **77 arquivo(s)** | **~32.689 linhas de codigo**

---

## RESUMO EXECUTIVO

- **Tipo de aplicacao:** Aplicacao Web Frontend (React)
- **Frontend / Stack principal:** React, TypeScript

**Para rodar o projeto:**
```bash
# Abra index.html no Preview (botao Play)
```

---

## ESTRUTURA DE ARQUIVOS

```
HTML/CSS/JS/
├── devmobile-fix/
│   ├── .github/
│   │   └── workflows/
│   │       ├── build-apk-eas.yml
│   │       └── build-apk-local.yml
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── app/
│   │   ├── (tabs)/
│   │   │   ├── _layout.tsx
│   │   │   ├── ai.tsx
│   │   │   ├── editor.tsx
│   │   │   ├── index.tsx
│   │   │   ├── plugins.tsx
│   │   │   ├── pwa.tsx
│   │   │   ├── settings.tsx
│   │   │   ├── tasks.tsx
│   │   │   └── terminal.tsx
│   │   ├── _layout.tsx
│   │   └── +not-found.tsx
│   ├── components/
│   │   ├── AIChat.tsx
│   │   ├── AIMemoryModal.tsx
│   │   ├── APKBuilderModal.tsx
│   │   ├── CampoLivreModal.tsx
│   │   ├── CheckpointsModal.tsx
│   │   ├── CodeEditor.tsx
│   │   ├── CombinarAppsModal.tsx
│   │   ├── DatabasePanel.tsx
│   │   ├── ErrorBoundary.tsx
│   │   ├── ErrorFallback.tsx
│   │   ├── FileSidebar.tsx
│   │   ├── FloatingAI.tsx
│   │   ├── GitHubModal.tsx
│   │   ├── HtmlPlayground.tsx
│   │   ├── KeyboardAwareScrollViewCompat.tsx
│   │   ├── LibrarySearch.tsx
│   │   ├── ManualModal.tsx
│   │   ├── MessageRenderer.tsx
│   │   ├── MonacoEditor.tsx
│   │   ├── PreviewPanel.tsx
│   │   ├── ProjectOverviewModal.tsx
│   │   ├── ProjectPlanModal.tsx
│   │   ├── SystemStatus.tsx
│   │   ├── Terminal.tsx
│   │   ├── VoiceAssistant.tsx
│   │   ├── VSCodeView.tsx
│   │   ├── VSCodeWebModal.tsx
│   │   └── XTermWebView.tsx
│   ├── constants/
│   │   └── colors.ts
│   ├── context/
│   │   └── AppContext.tsx
│   ├── data/
│   │   └── featuredProjects.ts
│   ├── hooks/
│   │   ├── useApiBase.ts
│   │   └── useColors.ts
│   ├── plugins/
│   │   └── withTermuxIntent.js
│   ├── server/
│   │   ├── templates/
│   │   │   └── landing-page.html
│   │   └── serve.js
│   ├── services/
│   │   ├── apiBase.ts
│   │   ├── githubService.ts
│   │   ├── localSQLite.ts
│   │   ├── previewService.ts
│   │   ├── runtimeMode.ts
│   │   ├── storageService.ts
│   │   └── terminalService.ts
│   ├── utils/
│   │   ├── projectPlan.ts
│   │   └── zipUtils.ts
│   ├── .easignore
│   ├── .env
│   ├── .env.example
│   ├── .gitignore
│   ├── .npmrc
│   ├── app.json
│   ├── babel.config.js
│   ├── capacitor.config.ts
│   ├── COMO_BUILDAR.md
│   ├── COMO-BUILDAR-APK.md
│   ├── eas.json
│   ├── expo-env.d.ts
│   ├── GERAR-APK.md
│   ├── metro.config.js
│   ├── package.json
│   ├── PLANO.md
│   └── tsconfig.json
└── MANUAL-GERAR-APK.html
```

---

## STACK TECNOLOGICO DETECTADO

- **Frontend:** React, TypeScript

---

## ROTAS DA API (endpoints detectados automaticamente)

```
POST   /api/chat  (em devmobile-fix/data/featuredProjects.ts)
GET    /api/saude  (em devmobile-fix/data/featuredProjects.ts)
POST   /api/chat  (em devmobile-fix/data/featuredProjects.ts)
GET    /api/saude  (em devmobile-fix/data/featuredProjects.ts)
POST   /api/chat  (em devmobile-fix/data/featuredProjects.ts)
GET    /api/saude  (em devmobile-fix/data/featuredProjects.ts)
POST   /api/chat  (em devmobile-fix/data/featuredProjects.ts)
GET    /api/provedores  (em devmobile-fix/data/featuredProjects.ts)
GET    /api/saude  (em devmobile-fix/data/featuredProjects.ts)
```

---

## VARIAVEIS DE AMBIENTE NECESSARIAS

Crie um arquivo `.env` na raiz com estas variaveis:

```env
PORT=seu_valor_aqui
GROQ_API_KEY=seu_valor_aqui
GROQ_MODEL=seu_valor_aqui
ANTHROPIC_API_KEY=seu_valor_aqui
CLAUDE_MODEL=seu_valor_aqui
GEMINI_API_KEY=seu_valor_aqui
GEMINI_MODEL=seu_valor_aqui
OPENAI_API_KEY=seu_valor_aqui
EXPO_PUBLIC_DOMAIN=seu_valor_aqui
BASE_PATH=seu_valor_aqui
EXPO_PUBLIC_API_BASE_URL=seu_valor_aqui
EXPO_PUBLIC_REMOTE_API_URL=seu_valor_aqui
EXPO_PUBLIC_APP_MODE=seu_valor_aqui
EXPO_PUBLIC_API_STRATEGY=seu_valor_aqui
EXPO_PUBLIC_LOCAL_API_PORT=seu_valor_aqui
EXPO_PUBLIC_LOCAL_PREVIEW_PORT=seu_valor_aqui
EXPO_PUBLIC_ENABLE_TERMUX=seu_valor_aqui
EXPO_PUBLIC_ENABLE_REMOTE_AI=seu_valor_aqui
EXPO_PUBLIC_ENABLE_GITHUB=seu_valor_aqui
EXPO_PUBLIC_ENABLE_REMOTE_DB=seu_valor_aqui
EXPO_PUBLIC_ENABLE_REMOTE_TERMINAL=seu_valor_aqui
```

---

## ARQUIVOS PRINCIPAIS

- `devmobile-fix/app/(tabs)/index.tsx` — Arquivo principal

---

## GUIA COMPLETO — O QUE CADA PARTE DO PROJETO FAZ

> Esta secao explica, em linguagem simples, o que e para que serve cada pasta e cada arquivo.

### 📁 Raiz do Projeto (pasta principal)
> Arquivos de configuracao e pontos de entrada ficam aqui.

**`MANUAL-GERAR-APK.html`** _(122 linhas)_
Arquivo HTML — parte do projeto.

---

### 📁 `devmobile-fix/`
> Pasta 'devmobile-fix' — agrupamento de arquivos relacionados.

**`.easignore`** _(25 linhas)_
Arquivo EASIGNORE — parte do projeto.

**`.env`** _(2 linhas)_
Arquivo de variaveis secretas (senhas, chaves de API). NUNCA suba este arquivo para o GitHub.

**`.env.example`** _(91 linhas)_
Arquivo de variaveis secretas (senhas, chaves de API). NUNCA suba este arquivo para o GitHub.

**`.gitignore`** _(42 linhas)_
Lista de arquivos/pastas que o Git deve IGNORAR (nao versionar). Ex: node_modules, .env

**`.npmrc`** _(3 linhas)_
Arquivo NPMRC — parte do projeto.

**`COMO-BUILDAR-APK.md`** _(78 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`COMO_BUILDAR.md`** _(113 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`GERAR-APK.md`** _(62 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`PLANO.md`** _(187 linhas)_
Este documento! Gerado automaticamente pelo SK Code Editor com toda a estrutura do projeto.

**`app.json`** _(63 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`babel.config.js`** _(7 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`capacitor.config.ts`** _(43 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`eas.json`** _(57 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`expo-env.d.ts`** _(3 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`metro.config.js`** _(28 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`package.json`** _(78 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(24 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `devmobile-fix/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(23 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `devmobile-fix/app/`
> Pasta 'app' — agrupamento de arquivos relacionados.

**`+not-found.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`_layout.tsx`** _(69 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

---

### 📁 `devmobile-fix/components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`AIChat.tsx`** _(1493 linhas)_
Componente de CHAT/MENSAGENS — interface de conversa em tempo real.

**`AIMemoryModal.tsx`** _(203 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`APKBuilderModal.tsx`** _(1058 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`CampoLivreModal.tsx`** _(989 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`CheckpointsModal.tsx`** _(173 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`CodeEditor.tsx`** _(383 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`CombinarAppsModal.tsx`** _(352 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`DatabasePanel.tsx`** _(887 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`ErrorBoundary.tsx`** _(55 linhas)_
Componente de ERRO — exibido quando algo da errado, com mensagem explicativa.

**`ErrorFallback.tsx`** _(279 linhas)_
Componente de ERRO — exibido quando algo da errado, com mensagem explicativa.

**`FileSidebar.tsx`** _(742 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`FloatingAI.tsx`** _(897 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`GitHubModal.tsx`** _(1257 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`HtmlPlayground.tsx`** _(706 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`KeyboardAwareScrollViewCompat.tsx`** _(30 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`LibrarySearch.tsx`** _(327 linhas)_
Componente de BUSCA — campo e logica para filtrar/encontrar conteudo.

**`ManualModal.tsx`** _(776 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`MessageRenderer.tsx`** _(504 linhas)_
Componente de CHAT/MENSAGENS — interface de conversa em tempo real.

**`MonacoEditor.tsx`** _(163 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`PreviewPanel.tsx`** _(500 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`ProjectOverviewModal.tsx`** _(504 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`ProjectPlanModal.tsx`** _(369 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`SystemStatus.tsx`** _(480 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Terminal.tsx`** _(1297 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`VSCodeView.tsx`** _(685 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`VSCodeWebModal.tsx`** _(363 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`VoiceAssistant.tsx`** _(991 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`XTermWebView.tsx`** _(311 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

---

### 📁 `devmobile-fix/constants/`
> Pasta 'constants' — agrupamento de arquivos relacionados.

**`colors.ts`** _(98 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `devmobile-fix/context/`
> Gerenciamento de estado global — dados compartilhados entre telas.

**`AppContext.tsx`** _(1382 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

---

### 📁 `devmobile-fix/data/`
> Pasta 'data' — agrupamento de arquivos relacionados.

**`featuredProjects.ts`** _(802 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `devmobile-fix/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`useApiBase.ts`** _(100 linhas)_
HOOK de dados — busca informacoes da API e gerencia estado de carregamento e erro.

**`useColors.ts`** _(25 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'colors'.

---

### 📁 `devmobile-fix/plugins/`
> Pasta 'plugins' — agrupamento de arquivos relacionados.

**`withTermuxIntent.js`** _(26 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `devmobile-fix/server/`
> Pasta 'server' — agrupamento de arquivos relacionados.

**`serve.js`** _(136 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `devmobile-fix/services/`
> Comunicacao com servidor, banco de dados ou APIs externas.

**`apiBase.ts`** _(28 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`githubService.ts`** _(530 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`localSQLite.ts`** _(81 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`previewService.ts`** _(17 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`runtimeMode.ts`** _(56 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`storageService.ts`** _(16 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`terminalService.ts`** _(29 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

---

### 📁 `devmobile-fix/utils/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`projectPlan.ts`** _(208 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`zipUtils.ts`** _(473 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `devmobile-fix/.github/workflows/`
> Pasta 'workflows' — agrupamento de arquivos relacionados.

**`build-apk-eas.yml`** _(72 linhas)_
Arquivo YML — parte do projeto.

**`build-apk-local.yml`** _(126 linhas)_
Arquivo YML — parte do projeto.

---

### 📁 `devmobile-fix/app/(tabs)/`
> Pasta '(tabs)' — agrupamento de arquivos relacionados.

**`_layout.tsx`** _(161 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

**`ai.tsx`** _(81 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`editor.tsx`** _(1403 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`index.tsx`** _(3958 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

**`plugins.tsx`** _(1234 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`pwa.tsx`** _(625 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`settings.tsx`** _(1886 linhas)_
Componente de CONFIGURACOES — tela onde o usuario ajusta preferencias do app.

**`tasks.tsx`** _(522 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`terminal.tsx`** _(213 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `devmobile-fix/server/templates/`
> Pasta 'templates' — agrupamento de arquivos relacionados.

**`landing-page.html`** _(461 linhas)_
Arquivo HTML — parte do projeto.

---

## CONTEXTO PARA IA (copie e cole para continuar o projeto)

> Use este bloco para explicar o projeto para qualquer IA ou desenvolvedor:

```
Projeto: HTML/CSS/JS
Tipo: Aplicacao Web Frontend (React)
Stack: React, TypeScript
Arquivos: 77 | Linhas: ~32.689
Rotas API: 9 endpoint(s) detectado(s)
Variaveis de ambiente necessarias: PORT, GROQ_API_KEY, GROQ_MODEL, ANTHROPIC_API_KEY, CLAUDE_MODEL, GEMINI_API_KEY, GEMINI_MODEL, OPENAI_API_KEY, EXPO_PUBLIC_DOMAIN, BASE_PATH, EXPO_PUBLIC_API_BASE_URL, EXPO_PUBLIC_REMOTE_API_URL, EXPO_PUBLIC_APP_MODE, EXPO_PUBLIC_API_STRATEGY, EXPO_PUBLIC_LOCAL_API_PORT, EXPO_PUBLIC_LOCAL_PREVIEW_PORT, EXPO_PUBLIC_ENABLE_TERMUX, EXPO_PUBLIC_ENABLE_REMOTE_AI, EXPO_PUBLIC_ENABLE_GITHUB, EXPO_PUBLIC_ENABLE_REMOTE_DB, EXPO_PUBLIC_ENABLE_REMOTE_TERMINAL

Estrutura principal:
  MANUAL-GERAR-APK.html
  devmobile-fix/.easignore
  devmobile-fix/.env
  devmobile-fix/.env.example
  devmobile-fix/.github/workflows/build-apk-eas.yml
  devmobile-fix/.github/workflows/build-apk-local.yml
  devmobile-fix/.gitignore
  devmobile-fix/.npmrc
  devmobile-fix/.replit-artifact/artifact.toml
  devmobile-fix/COMO-BUILDAR-APK.md
  devmobile-fix/COMO_BUILDAR.md
  devmobile-fix/GERAR-APK.md
  devmobile-fix/PLANO.md
  devmobile-fix/app.json
  devmobile-fix/app/(tabs)/_layout.tsx
  devmobile-fix/app/(tabs)/ai.tsx
  devmobile-fix/app/(tabs)/editor.tsx
  devmobile-fix/app/(tabs)/index.tsx
  devmobile-fix/app/(tabs)/plugins.tsx
  devmobile-fix/app/(tabs)/pwa.tsx
  devmobile-fix/app/(tabs)/settings.tsx
  devmobile-fix/app/(tabs)/tasks.tsx
  devmobile-fix/app/(tabs)/terminal.tsx
  devmobile-fix/app/+not-found.tsx
  devmobile-fix/app/_layout.tsx
  devmobile-fix/babel.config.js
  devmobile-fix/capacitor.config.ts
  devmobile-fix/components/AIChat.tsx
  devmobile-fix/components/AIMemoryModal.tsx
  devmobile-fix/components/APKBuilderModal.tsx
  devmobile-fix/components/CampoLivreModal.tsx
  devmobile-fix/components/CheckpointsModal.tsx
  devmobile-fix/components/CodeEditor.tsx
  devmobile-fix/components/CombinarAppsModal.tsx
  devmobile-fix/components/DatabasePanel.tsx
  devmobile-fix/components/ErrorBoundary.tsx
  devmobile-fix/components/ErrorFallback.tsx
  devmobile-fix/components/FileSidebar.tsx
  devmobile-fix/components/FloatingAI.tsx
  devmobile-fix/components/GitHubModal.tsx
  devmobile-fix/components/HtmlPlayground.tsx
  devmobile-fix/components/KeyboardAwareScrollViewCompat.tsx
  devmobile-fix/components/LibrarySearch.tsx
  devmobile-fix/components/ManualModal.tsx
  devmobile-fix/components/MessageRenderer.tsx
  devmobile-fix/components/MonacoEditor.tsx
  devmobile-fix/components/PreviewPanel.tsx
  devmobile-fix/components/ProjectOverviewModal.tsx
  devmobile-fix/components/ProjectPlanModal.tsx
  devmobile-fix/components/SystemStatus.tsx
  devmobile-fix/components/Terminal.tsx
  devmobile-fix/components/VSCodeView.tsx
  devmobile-fix/components/VSCodeWebModal.tsx
  devmobile-fix/components/VoiceAssistant.tsx
  devmobile-fix/components/XTermWebView.tsx
  devmobile-fix/constants/colors.ts
  devmobile-fix/context/AppContext.tsx
  devmobile-fix/data/featuredProjects.ts
  devmobile-fix/eas.json
  devmobile-fix/expo-env.d.ts
  devmobile-fix/hooks/useApiBase.ts
  devmobile-fix/hooks/useColors.ts
  devmobile-fix/metro.config.js
  devmobile-fix/package.json
  devmobile-fix/plugins/withTermuxIntent.js
  devmobile-fix/server/serve.js
  devmobile-fix/server/templates/landing-page.html
  devmobile-fix/services/apiBase.ts
  devmobile-fix/services/githubService.ts
  devmobile-fix/services/localSQLite.ts
  devmobile-fix/services/previewService.ts
  devmobile-fix/services/runtimeMode.ts
  devmobile-fix/services/storageService.ts
  devmobile-fix/services/terminalService.ts
  devmobile-fix/tsconfig.json
  devmobile-fix/utils/projectPlan.ts
  devmobile-fix/utils/zipUtils.ts
```

---

*Plano gerado pelo SK Code Editor — 14/05/2026, 14:51:10*