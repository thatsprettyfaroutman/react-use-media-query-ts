# react-use-media-query-ts

React hook for matching media queries. For example you can use it for detecting dark mode or changes in viewport width breakpoints. Written in Typescript.

## Setup

```
npm i react-use-media-query-ts
```

## Usage

```jsx
import useMediaQuery from 'react-use-media-query-ts'

function App() {
  const darkMode = useMediaQuery('(prefers-color-scheme: dark)')
  const mobile = useMediaQuery('(max-width: 768px)')

  const style = { color: darkMode ? 'white' : 'black' }

  return (
    <div style={style}>
      Seems like you're {!mobile && <strong>not</strong>} using a mobile device
    </div>
  )
}
```

## Example

https://kymdg1-5173.csb.app/

## License

MIT
