Repro case for https://github.com/Microsoft/TypeScript/issues/12814

To run, `npm install && ./node_modules/typescript/bin/tsc -p ./tsconfig.json`

Output:
```
node_modules/@types/es6-promise/index.d.ts(11,15): error TS2300: Duplicate identifier 'Promise'.
node_modules/@types/es6-promise/index.d.ts(42,19): error TS2300: Duplicate identifier 'Promise'.
node_modules/typescript/lib/lib.es6.d.ts(4936,11): error TS2300: Duplicate identifier 'Promise'.
node_modules/typescript/lib/lib.es6.d.ts(5261,11): error TS2300: Duplicate identifier 'Promise'.
node_modules/typescript/lib/lib.es6.d.ts(5511,13): error TS2300: Duplicate identifier 'Promise'.
node_modules/typescript/lib/lib.es6.d.ts(5737,11): error TS2300: Duplicate identifier 'Promise'.
```
