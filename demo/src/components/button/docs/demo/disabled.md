---
order: 3
title: 不可用状态
component: Button
---

添加 `disabled` 属性即可让按钮处于不可用状态，同时按钮样式也会改变。

```JS DEMO
import { Button } from 'antd';
import React from 'react';
export default class extends React.Component {
  render() {
    return <div>
      <Button type="primary">Primary</Button>
      <Button type="primary" disabled>
        Primary(disabled)
      </Button>
      <br />
      <Button>Default</Button>
      <Button disabled>Default(disabled)</Button>
      <br />
      <Button type="dashed">Dashed</Button>
      <Button type="dashed" disabled>
        Dashed(disabled)
      </Button>
      <br />
      <Button type="link">Link</Button>
      <Button type="link" disabled>
        Link(disabled)
      </Button>
      <br />
      <Button type="link" danger>
        Danger Link
      </Button>
      <Button type="link" danger disabled>
        Danger Link(disabled)
      </Button>
      <br />
      <Button danger>Danger Default</Button>
      <Button danger disabled>
        Danger Default(disabled)
      </Button>
      <div className="site-button-ghost-wrapper">
        <Button ghost>Ghost</Button>
        <Button ghost disabled>
          Ghost(disabled)
        </Button>
      </div>
    </div>
  }
}
```