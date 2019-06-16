# react-use-window-size

[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors)

[![Version](https://badge.fury.io/js/%40alemesa%2Freact-use-window-size.svg)](https://badge.fury.io/js/%40alemesa%2Freact-use-window-size)
[![MIT license](http://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT)
![Size](https://img.shields.io/bundlephobia/min/@alemesa/react-use-window-size.svg)

[![NPM](https://nodeico.herokuapp.com/@alemesa/react-use-window-size.svg)](https://npmjs.com/package/@alemesa/react-use-window-size)

[React Hook](https://reactjs.org/docs/hooks-intro.html) that uses the window size

#### Usage

```bash
npm i @alemesa/react-use-window-size
```

---

- Example Codesanbox:

[![Edit react-use-window-size](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/wizardly-microservice-koxej?fontsize=14)

---

- Simple Example:
  Check Window Size

```javascript
import React, { useRef, useEffect } from "react";
import useWindowSize from "@alemesa/react-use-window-size";

const Header = React.memo(() => {
  // Pass a reference to the custom hook
  // Set the debounce to 100ms - would be 250 by default
  const windowSize = useWindowSize(100);

  useEffect(() => {
    if (windowSize.innerWidth > 1000) {
      // Bigger than 1000px
      console.log("bigger than 1000px");
    }
  }, [windowSize]);

  return <h3>Example</h3>;
});

export default Header;
```

## Contributors

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table><tr><td align="center"><a href="https://alemesa.com"><img src="https://avatars3.githubusercontent.com/u/14832910?v=4" width="100px;" alt="Alejandro Mesa"/><br /><sub><b>Alejandro Mesa</b></sub></a><br /><a href="#infra-alemesa" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/alemesa/react-use-window-size/commits?author=alemesa" title="Code">💻</a></td></tr></table>

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
