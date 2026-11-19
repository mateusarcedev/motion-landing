# MOTION Studio — Landing

Site público do MOTION Studio: https://motion.mateusarce.dev

- `page.template.html`, `case*.template.html`, `gallery_data.py`: fonte do site.
- `build.py`: gera `site/` (pt-BR e `en/`). Rode `python3 build.py` após editar os templates.
- `site/`: saída publicada pela Vercel (Root Directory = `site`). É versionada, incluindo vídeos e imagens.
- `serve.mjs`: servidor local para preview; `test_*.mjs`: testes de frontend, galeria e publicação.

Os vídeos e imagens em `site/videos` e `site/assets` vêm dos renders feitos no monorepo
[motion-studio](https://github.com/mateusarcedev/motion-studio). Quando um render novo for aprovado, copie o
arquivo para cá e faça commit.
