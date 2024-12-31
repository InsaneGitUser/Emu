---
title: gb
---

A shortcut method for `Nostalgist.launch` method, with some additional default options for GB emulation.

It will use `mgba` as the default core for emulation.

## Usage
Basic usage:
```js
await Nostalgist.gb('blastah.gb')

// is equal to
await Nostalgist.launch({ core: 'mgba', rom: 'blastah.gb' })
```

## Arguments
+ ### `options`
  **type:** `string | Object`

  If the `options` is a `string | File | { fileName: string; fileContent: Blob }`, it will be treated as `{ rom: options }` in fact.

  If the `options` is an `Object`, then it is the same as the `options` argument for `Nostalgist.launch`.

  Please refer to [launch#options](/apis/launch/#options).
