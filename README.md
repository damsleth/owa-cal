# owa-cal (archived)

Active development continues at [damsleth/owa-tools](https://github.com/damsleth/owa-tools).

This repository is archived and read-only. The full history of `owa-cal` is preserved under `owa_cal/` in the consolidated monorepo via subtree merge - `git log owa_cal/` in `owa-tools` walks every commit from this repo.

## Why

`owa-cal`, `owa-mail`, `owa-graph`, `owa-doctor`, `owa-drive`, `owa-people`, and `owa-sched` were all stdlib-only consumers of `owa-piggy`'s access tokens with substantial duplicated code (auth bridge, JWT decode, atomic config writes, formatting helpers). One repo with `owa_core` as the shared library replaces seven copies of each concern. `owa-piggy` itself remains a separate repository.

## Install

```sh
pipx install owa-tools
```

The `owa-cal` binary is unchanged.
