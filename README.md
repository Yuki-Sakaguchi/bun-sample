# Bun を試してみる

https://bun.sh/

## インストール
```bash
curl -fsSL https://bun.sh/install | bash
```

## index.tsx
```tsx
const server = Bun.serve({
  port: 3000,
  fetch(request) {
    return new Response("Welcome to Bun!");
  },
});

console.log(`Listening on localhost:${server.port}`);
```

## 実行
```bash
bun index.tsx
```
