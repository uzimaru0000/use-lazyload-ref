# use-lazyload-ref

![CI Status](https://github.com/saitoeku3/use-lazyload-ref/workflows/Node%20CI/badge.svg)

> A custom hook to use lazy load easily


## Install

```
$ npm install use-lazyload-ref
$ yarn add use-lazyload-ref
```

## Usage

```tsx
import React from 'react'
import useLazyloadRef from 'use-lazyload-ref'

const Component = ({ url }) => {
  const [ref, isLoaded] = useLazyloadRef()

  return (
    <>
      {isLoaded || <Skeleton />}
      <img ref={ref} data-src={url}>
    <>
  )
}
```

## License

MIT © saitoeku3
