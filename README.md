
# colors

## Install

```sh
~$ npm i @song940/colors --save
```

## Example

```javascript
import { green, italic } from "@song940/colors";

console.log(green(`How are ${italic(`you`)} doing?`));
```

## Benchmarks

`nanocolors` [benchmark](https://github.com/ai/nanocolors/tree/main/test):

```diff
./test/size.js
Data from packagephobia.com
chalk         101 kB
cli-color    1249 kB
ansi-colors    25 kB
kleur          21 kB
colorette      16 kB
nanocolors     16 kB
+picocolors     8 kB
```

```diff
$ ./test/complex-benchmark.js
chalk          2,618,824 ops/sec
cli-color        326,445 ops/sec
ansi-colors    1,057,188 ops/sec
kleur          2,543,659 ops/sec
kleur/colors   2,841,679 ops/sec
colorette      3,219,038 ops/sec
nanocolors     3,672,600 ops/sec
+picocolors    6,079,950 ops/sec
```

`colorette` [benchmark](https://github.com/jorgebucaran/colorette/tree/main/bench):

```diff
$ npm start
+picocolors × 1,203,773 ops/sec
chalk × 474,359 ops/sec
kleur × 482,915 ops/sec
colors × 233,138 ops/sec
colorette × 657,896 ops/sec
nanocolors × 660,817 ops/sec
ansi-colors × 290,986 ops/sec
```