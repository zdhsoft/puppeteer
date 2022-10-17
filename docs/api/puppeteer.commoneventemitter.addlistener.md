---
sidebar_label: CommonEventEmitter.addListener
---

# CommonEventEmitter.addListener() method

To maintain parity with the built in NodeJS event emitter which uses
removeListener rather than `off`. If you're implementing new code you should use
`off`.

**Signature:**

```typescript
interface CommonEventEmitter {
  addListener(event: EventType, handler: Handler): CommonEventEmitter;
}
```

## Parameters

| Parameter | Type                                  | Description |
| --------- | ------------------------------------- | ----------- |
| event     | [EventType](./puppeteer.eventtype.md) |             |
| handler   | [Handler](./puppeteer.handler.md)     |             |

**Returns:**

[CommonEventEmitter](./puppeteer.commoneventemitter.md)
