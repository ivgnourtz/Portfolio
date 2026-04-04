---
title: Getting Started with TypeScript
tags:
  - typescript
  - programming
  - tutorial
date: 2026-04-01
---

## TypeScript là gì?

TypeScript là một ngôn ngữ lập trình mã nguồn mở được phát triển bởi Microsoft. Nó là một superset của JavaScript, bổ sung thêm hệ thống kiểu tĩnh.

## Tại sao nên dùng TypeScript?

- **Phát hiện lỗi sớm:** Kiểm tra kiểu tại compile time
- **IDE hỗ trợ tốt hơn:** Autocomplete, refactoring, navigation
- **Code dễ bảo trì:** Type annotations giúp code self-documenting
- **Tương thích JavaScript:** Có thể dùng thư viện JS hiện có

## Cài đặt

```bash
npm install -g typescript
```

Kiểm tra phiên bản:

```bash
tsc --version
```

## Ví dụ cơ bản

```typescript
// Khai báo kiểu
function greet(name: string): string {
  return `Hello, ${name}!`;
}

// Interface
interface User {
  id: number;
  name: string;
  email: string;
}

// Type Union
type Status = "active" | "inactive" | "pending";
```

## Compile TypeScript

```bash
tsc index.ts
```

File `index.ts` sẽ được compile thành `index.js`.

---

> Xem thêm: [[notes]]
