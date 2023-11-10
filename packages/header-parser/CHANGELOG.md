# @definitelytyped/header-parser

## 0.0.186

### Patch Changes

- a18ce6b1: Remove use of module resolution and OTHER_FILES, instead include all dts files in packages

  Files in packages are no longer determined by import resolution stemming from `index.d.ts` and tests (along with those listed in `OTHER_FILES.txt`).
  Instead, all files matching the glob `**/*.d.{ts,cts,mts,*.d.ts}` are included in the package, excluding those inside of versioned subdirectories.

  While not used for automated package publishing, an `.npmignore` is now required in each package.
  This allows for one-off `npm pack`-ing of packages, such that external tooling can get a rough approximation of what will be published for analysis.

- Updated dependencies [a18ce6b1]
  - @definitelytyped/utils@0.0.184

## 0.0.185

### Patch Changes

- Updated dependencies [90e1d0ae]
  - @definitelytyped/typescript-versions@0.0.180
  - @definitelytyped/utils@0.0.183

## 0.0.184

### Patch Changes

- f9e73605: Remove validation of `"pnpm"` field

## 0.0.183

### Patch Changes

- Updated dependencies [2b3138a0]
  - @definitelytyped/utils@0.0.182

## 0.0.182

### Patch Changes

- Updated dependencies [97f68d6e]
  - @definitelytyped/utils@0.0.181

## 0.0.181

### Patch Changes

- Updated dependencies [d01cacd5]
  - @definitelytyped/utils@0.0.180

## 0.0.180

### Patch Changes

- 22ffaadf: Always convert contributor githubUsername to url (missing changeset)

## 0.0.179

### Patch Changes

- 024c3e73: Update @definitelytyped for Definitely Typed's monorepo upgrade
- Updated dependencies [024c3e73]
- Updated dependencies [9fffa8ff]
  - @definitelytyped/typescript-versions@0.0.179
  - @definitelytyped/utils@0.0.179