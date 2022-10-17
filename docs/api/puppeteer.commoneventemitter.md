---
sidebar_label: CommonEventEmitter
---

# CommonEventEmitter interface

**Signature:**

```typescript
export interface CommonEventEmitter
```

## Methods

| Method                                                                             | Description                                                                                                                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [addListener(event, handler)](./puppeteer.commoneventemitter.addlistener.md)       | To maintain parity with the built in NodeJS event emitter which uses removeListener rather than <code>off</code>. If you're implementing new code you should use <code>off</code>. |
| [emit(event, eventData)](./puppeteer.commoneventemitter.emit.md)                   |                                                                                                                                                                                    |
| [listenerCount(event)](./puppeteer.commoneventemitter.listenercount.md)            |                                                                                                                                                                                    |
| [off(event, handler)](./puppeteer.commoneventemitter.off.md)                       |                                                                                                                                                                                    |
| [on(event, handler)](./puppeteer.commoneventemitter.on.md)                         |                                                                                                                                                                                    |
| [once(event, handler)](./puppeteer.commoneventemitter.once.md)                     |                                                                                                                                                                                    |
| [removeAllListeners(event)](./puppeteer.commoneventemitter.removealllisteners.md)  |                                                                                                                                                                                    |
| [removeListener(event, handler)](./puppeteer.commoneventemitter.removelistener.md) |                                                                                                                                                                                    |
