
# supertokens-feat-783

A test repo for supertokens-node feature 783 to test the import for cjs, esm and typescript import fix


## Testing imports

```bash
  cd supertokens-node //main supertokens-node repo from my branch
  npm run build
  npm link
```

### For esm import check
As in the package.json I have added **type:module** so this directory will be able to import with import statement or esm imports

```bash
  cd test-import-esm
  npm link supertokens-node
  npm start
```
### For cjs import check
This is cjs directory will be able to import with require keyword.

```bash
  cd test-import-cjs
  npm link supertokens-node
  npm start
```
### For typescript import check
This is for typescript as we are also providing types for the directories we need to check for the same as well.

I have added scripts for both development and production.

```bash
  cd test-import-typescript
  npm link supertokens-node
  npm run start:dev // for development mode
  npm run build
  npm run start:prod // for production mode
```