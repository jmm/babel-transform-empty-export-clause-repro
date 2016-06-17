<!-- Related issue: http://example.com/123 -->

```sh
$ git clone {{thisRepo}}
$ cd {{thisRepoDir}}
$ git checkout {{thisBranch}}
$ npm i
$ npm run repro
```

# Expected result

Output in `dist/actual.js` should be free of ES module syntax and should have no exports other than the automatic `__esModule`.

# Actual result

Output still contains input: `export {};`.
