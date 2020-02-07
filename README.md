# Enzyme `parent` BUG

This is a bug with `.parent()` of `enzyme`.

```bash
yarn
yarn test
## Outputs:
# console.log src/__tests__/Foo-test.js:28
#     null  ----> This is not expected.

#   console.log src/__tests__/Foo-test.js:34
#     <div class="foo">Bar<div class="bar"></div></div>
```

My deps:

```json
// devDep
"enzyme": "^3.11.0",
"enzyme-adapter-react-16": "^1.15.2",
// dep
"react": "^16.10.2",
"react-dom": "^16.10.2",
```
