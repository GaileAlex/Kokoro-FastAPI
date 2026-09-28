# My Kokoro-FastAPI fork

Original: https://github.com/remsky/Kokoro-FastAPI (remote `upstream`).
My RTX 50 changes (cu128, CUDA 12.9.1, `kokoro-net` network) sit as a commit on top of the `release` branch.

## Updating to a new Kokoro release

Terminal:

```bash
git pull upstream release
git push
```

IntelliJ IDEA:

1. Git → Pull... → pick `upstream` in the remote list, branch `release` → Pull
2. Git → Push (Ctrl+Shift+K) → Push

On a conflict, keep my CUDA/cu128/network values and take everything else from the new version.

