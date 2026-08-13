# iOS 16 legacy migration closure

Recorded: 2026-08-13

## Claim and scope

Question: can the complete ordinary iOS 16 payload set in frozen legacy commit
`d881e84676308404c6947d0218c11f347a6f3a89` be copied exactly into this
archive shard and later cataloged with immutable provenance?

- First lifecycle stage: select the two ordinary iOS 16 roots in the frozen
  census whose same-device IPSW inputs use the iOS 16 (`20*`) build train.
- Last lifecycle stage: catalog entries independently verify both source trees
  against this shard's merged default-branch commit.
- Supported claim after closure: the two named Git subtrees were faithfully
  migrated and cataloged.
- Excluded: generating missing release history, interpreting README-only output
  as proof of no firmware changes, and resolving other census exceptions.

## Authority map

| Property | Authority |
| --- | --- |
| Frozen migration membership | Catalog census at the pinned legacy commit |
| Versions, builds, devices, and inputs | Strictly parsed source READMEs |
| Files, bytes, modes, and trees | Git objects at the pinned legacy commit |
| Destination payloads and manifests | Reviewed specs plus atomic batch staging |
| Catalog destination pins | Merged shard default-branch commit |

## Closure matrix

| Stage | Evidence | Status before publication |
| --- | --- | --- |
| Selection and trigger | Exactly two ordinary iOS 16 census roots | Closed |
| Inputs and resources | Both rows contain two `iPhone10,3,iPhone10,6` IPSW inputs | Closed |
| Transformation | Atomic staging and independent revalidation reproduce both payload trees | Closed |
| Advertisement and options | Generated shard README lists exactly two comparisons | Closed |
| Dispatch and transport | One unsigned shard commit and pull request | Unresolved |
| State transition | Shard merge precedes catalog publication | Unresolved |
| Outcome oracle | Catalog audit matches source and merged destination | Unresolved |

## Expected and observed inventory

| Source path | Files | Logical bytes | Git tree |
| --- | ---: | ---: | --- |
| `16_7_13_20H365__vs_16_7_14_20H370` | 1 | 557 | `2442f3cdd9416a5e89b3cfd4d46cd88030b22db6` |
| `16_7_14_20H370__vs_16_7_15_20H380` | 1 | 10,678 | `52ef7212cfd8353d38f0f74f3da1cc48911c341f` |

The complete batch contains 2 payload files and 11,235 logical bytes. Atomic
staging produced root tree `a7a6d7413d0521c9a22b9f22508229e7fabac68c`
for the initial shard plus both payloads and manifests.

## Negative-evidence audit and stop conditions

The absence of other ordinary iOS 16 rows is scoped to the frozen census; it
does not claim a complete Apple release history. Both payloads are README-only,
which proves their Git inventory but not that the generator observed every
possible firmware change. Stop if membership, README metadata, source trees,
batch inventory, staged scope, destination merge commit, or catalog audit
differs.

## Review-time bounded conclusion

Selection, input validation, atomic staging, independent revalidation, and
archive advertisement are closed. Publication, merged destination state, and
catalog verification remain unresolved until their GitHub transitions occur.
