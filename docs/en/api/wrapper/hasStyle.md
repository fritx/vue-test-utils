# hasStyle(style, value)

- **Arguments:**
  - `{string} style`
  - `{string} value`

- **Returns:** `{boolean}`

- **Usage:**

Assert `Wrapper` DOM node has style matching value

Returns `true` if `Wrapper` DOM node has `style` matching `string`.

**Note will only detect inline styles when running in `jsdom`.**

```js
import { mount } from 'vue-test-utils'
import { expect } from 'chai'
import Foo from './Foo.vue'

const wrapper = mount(Foo)
expect(wrapper.hasStyle('color', 'red')).to.equal(true)
```