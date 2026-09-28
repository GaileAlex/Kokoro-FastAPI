# Мой форк Kokoro-FastAPI

Оригинал: https://github.com/remsky/Kokoro-FastAPI (remote `upstream`).
Мои правки для RTX 50 (cu128, CUDA 12.9.1, сеть `kokoro-net`) лежат коммитом поверх ветки `release`.

## Обновление до новой версии Kokoro

Терминал:

```bash
git pull upstream release
git push
```

IntelliJ IDEA:

1. Git → Pull... → в списке remote выбери `upstream`, ветку `release` → Pull
2. Git → Push (Ctrl+Shift+K) → Push

Если git пишет "conflict", оставить мои значения CUDA/cu128/сети, остальное взять из новой версии.

## Не делать

Не включать Actions в форке (кнопка "I understand my workflows..."): push в `release` запустит workflow публикации.
