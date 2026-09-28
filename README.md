# libcups

xlings payload repacked from upstream binaries (conda-forge / Debian) by
[`.agents/tools/repack/repack.py`](https://github.com/openxlings/xim-pkgindex/tree/main/.agents/tools/repack).
Recipe: [`xim-pkgindex`](https://github.com/openxlings/xim-pkgindex) `pkgs/l/libcups.lua`.

Every release asset carries `PROVENANCE.md` (upstream artefacts, sha256, the exact command) and a `.sha256` sidecar.

## Sources

| artefact | sha256 | origin |
|---|---|---|
| https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h7a8fb5f_6.conda | `205c4f19550f3647832ec44e35e6d93c8c206782bdd620c1d7cf66237580ff9c` | conda-forge libcups 2.3.3 h7a8fb5f_6 (Apache-2.0) |

## Command

```
.agents/tools/repack/repack.py \
    --name libcups \
    --version 2.3.3 \
    --arch x86_64 \
    --src https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h7a8fb5f_6.conda#205c4f19550f3647832ec44e35e6d93c8c206782bdd620c1d7cf66237580ff9c \
    --drop 'lib/cups/*' \
    --host 'lib/libcups.so*' \
    --require lib/libcups.so.2 \
    --require lib/libcupsimage.so.2
```

