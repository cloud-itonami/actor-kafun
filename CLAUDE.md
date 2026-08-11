# cloud-itonami/actor-kafun

Canonical repository: `https://github.com/cloud-itonami/actor-kafun`.
The former `etzhayyim/com-etzhayyim-kafun` path is a compatibility redirect.

`kafun`（花粉）は花粉負荷を生態系の restoration route に整流する actor です。
旧 `etzhayyim/root/20-actors/kafun` の実装と契約はこの flat west project が所有します。

## Repository contract

- metadata、identity、dependency、ontology、lexicon、seed は EDN canonical。
- source は `src/kafun/`、test は `test/kafun/`。
- JSON/JSON-LD は外部 wire のみ。Go/TinyGo と shell runner は deprecated。
- G1 restoration-only、G2 map-not-cut-list、G3 consent、G4 carbon balance、
  G5 assessment-only、G6 no-server-key/no-network を維持する。

## Test

    bb run_tests.clj
    clojure -M:test

Mesh entry is `src/kafun/mesh.clj`; canonical seed is `data/seed.edn`.
