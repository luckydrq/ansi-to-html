# luckydrq-ansi-to-html

Forked from [rburns/ansi-to-html](https://github.com/rburns/ansi-to-html).

Main difference: `options.escapeXML` support passed in a function to allow custumizing your own escape behavior. That is:

Change

```typescript
escapeXML?: boolean
```

to

```typescript
escapeXML?: boolean | ((text: string) => string);
```
