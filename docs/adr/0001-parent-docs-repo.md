---
status: accepted
---

# Parent repo holds design docs; Unity game added later as a sibling

This repo is the parent. It currently holds only the design docs (in `docs/`); the
Unity project is added later as a **sibling** folder, not nested under `docs/`. We
chose this over starting a code+docs monorepo now so the docs can mature first and
the game project drops in clean. Until it exists, page "Code" sections stay
placeholders.
