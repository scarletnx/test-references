# edenprobe

How each case of Amberlith (edenprobe before 1.0.0) ends on ScarletNX, a run's baseline: `# build:` and `# mode:`,
then one case a line, `suite: name` for one that passes and `[RESULT] suite: name` for one that ends otherwise
(ScarletNX's `docs/dev/edenprobe.md`).

- `linux-x86_64.txt`: the pinned NRO's, which ScarletNX's CI (`scripts/ci/linux.sh amberlith_run`) and its
  `edenprobe_vk_memory_*` tests hold each run to, and which Amberlith's nightly is compared with as advice.
- `android-x86_64.txt`: the pinned APK's, as CI runs it.
- `compute-readback.txt`: the `edenprobe_compute_readback` test's, the wimsy suite's heavy level.

Written by `scripts/edenprobe.py baseline RUN/baseline.txt... -o <this folder>/<file>` from runs of one build and one
mode: a new Amberlith release is a commit here and the new pin in ScarletNX's `cpmfile.json`, in the pull request that
pins the release.
