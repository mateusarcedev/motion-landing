# MOTION Studio — Landing

Site público do MOTION Studio: https://motion.mateusarce.dev

```
src/       templates HTML, dados da galeria (gallery_data.py), og.html, wave.txt
scripts/   build.py (gera site/), build_og.mjs (imagens OG), serve.mjs (preview local)
tests/     testes Playwright: frontend, galeria, publicação
site/      saída publicada pela Vercel (Root Directory = site), versionada com vídeos e imagens
docs/      BRIEF, manifesto da entrega v1 e o deck original (slides/)
reviews/   resultados de QA (.json/.md versionados; screenshots ignorados)
```

## Uso

```bash
npm install          # playwright-core (usa o Chromium em ~/.cache/ms-playwright)
npm run build        # templates em src/ -> site/
npm run serve        # http://localhost:3388
npm test
```

Os vídeos e imagens em `site/videos` e `site/assets` vêm dos renders feitos no monorepo
[motion-studio](https://github.com/mateusarcedev/motion-studio). Quando um render novo for aprovado, copie o
arquivo para cá e faça commit.
