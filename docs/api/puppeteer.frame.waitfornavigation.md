---
sidebar_label: Frame.waitForNavigation
---

# Frame.waitForNavigation() method

Like [Page.waitForNavigation()](./puppeteer.page.waitfornavigation.md), but on this frame.

**Signature:**

```typescript
class Frame {
  waitForNavigation(options?: WaitForOptions): Promise<HTTPResponse | null>;
}
```

## Parameters

| Parameter | Type                                            | Description       |
| --------- | ----------------------------------------------- | ----------------- |
| options   | [WaitForOptions](./puppeteer.waitforoptions.md) | <i>(Optional)</i> |

**Returns:**

Promise&lt;[HTTPResponse](./puppeteer.httpresponse.md) \| null&gt;
