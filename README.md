# nx-move-reexports

Simple repo to reproduce NX Move Generator which does not update reexports

## Reproduction Instructions

- Clone Repository
- Run `npx nx generate @nx/workspace:move --destination=libs/foo/util-moved --projectName=util --newProjectName=util --importPath=@my-org/foo-util-moved --projectNameAndRootFormat=as-provided --no-interactive`
- `libs/shell/src/lib/shell.ts` is updated
- `libs/shell/src/index.ts` **is Not Updated**
