[![npm version](https://img.shields.io/npm/v/react-mobile-console.svg?color=blue)](https://www.npmjs.com/package/react-mobile-console) [![npm downloads](https://img.shields.io/npm/dm/react-mobile-console.svg?color=brightgreen)](https://www.npmjs.com/package/react-mobile-console) [![GitHub stars](https://img.shields.io/github/stars/teniryte/react-mobile-console?style=social)](https://github.com/teniryte/react-mobile-console) [![License](https://img.shields.io/github/license/teniryte/react-mobile-console)](LICENSE)

# react-mobile-console

A lightweight, debug console component for React applications that provides an external debugging interface similar to browser developer tools. Perfect for mobile development, testing, and debugging React apps in various environments.

<a href="https://mobile-console.teniryte.ru">Open Demo</a>

## How it works:

> When the component mounts, the global `console` object methods (`log`, `info`, `debug`, `time`, `timeEnd`) are replaced with MobileConsole methods. When the component unmounts, the original methods are restored. **Only for dev and test environments**!

## Features

- 🚀 **External Debug Console** - Overlay console that doesn't interfere with your app's UI
- 📱 **Mobile-Friendly** - Optimized for mobile devices with touch-friendly interface
- 🔧 **Interactive REPL** - Execute JavaScript code directly in the console
- 💾 **Global Temp Storage** - Save objects to global scope when clicked (like devtools)
- 🛡️ **Failsafe Stringification** - Safe stringification of all values

<table>
<tr>
<td width="33%" valign="top">
<img src="https://cdn.teniryte.ru/img/mobile-console/1.jpg" width="500">
</td>
<td width="33%" valign="top">
<img src="https://cdn.teniryte.ru/img/mobile-console/2.jpg" width="500">
</td>
<td width="33%" valign="top">
<img src="https://cdn.teniryte.ru/img/mobile-console/3.jpg" width="500">
</td>
</tr>
</table>


## Installation

```bash
npm install react-mobile-console
# or
yarn add react-mobile-console
```

## Quick Start

```tsx
import { MobileConsole } from 'react-mobile-console';

function App() {
  return (
    <>
      <MobileConsole onClose={() => setShowConsole(false)} />
    </>
  );
}
```

## License

MIT © [teniryte](https://github.com/teniryte)
