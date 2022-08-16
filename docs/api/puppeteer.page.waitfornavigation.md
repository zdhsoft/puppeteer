---
sidebar_label: Page.waitForNavigation
---

# Page.waitForNavigation() method

Waits for the page to navigate to a new URL or reload. It is useful when you run code that will indirectly cause the page to navigate.

Usage of the [History API](https://developer.mozilla.org/en-US/docs/Web/API/History_API) to change the URL is considered a navigation.

**Signature:**

```typescript
class Page {
  waitForNavigation(options?: WaitForOptions): Promise<HTTPResponse | null>;
}
```

## Parameters

| Parameter | Type                                            | Description                                                  |
| --------- | ----------------------------------------------- | ------------------------------------------------------------ |
| options   | [WaitForOptions](./puppeteer.waitforoptions.md) | <i>(Optional)</i> options to configure the waiting behavior. |

**Returns:**

Promise&lt;[HTTPResponse](./puppeteer.httpresponse.md) \| null&gt;

A promise which resolves to the main resource response of the navigation.

- In case of multiple redirects, the navigation will resolve with the response of the last redirect. - In case of navigation to a different anchor or navigation due to History API usage, the navigation will resolve with `null`.

## Example

```ts
const [response] = await Promise.all([
  // The navigation promise resolves after navigation has finished
  page.waitForNavigation(),
  // Clicking the link will indirectly cause a navigation
  page.click('a.my-link'),
]);
```
