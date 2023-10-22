# sh-snippets README

This snippets is for oriental-salad team. It is used for creating a new file with a template.

## Use for

1. Typescript
2. React Functional Component
3. Next.js 13+ app router
4. Tailwindcss
5. Zustand
6. Jest

## Snippets

### orct - Common Type

```typescript
// file name: test.ts
export type test = ;
```

### orci - Common Interface

```typescript
// file name: test.ts
export interface test {}
```

### orcuf - Common Util Fnc

```typescript
// file name: test.ts
export const test = () => {};
```

### orch - Common hook

```typescript
// file name: test.tsx
export const test = () => {};
```

### orcc - Common Constant

```typescript
// file name: test.tsx
export const test = {};
```

### orzsd - Zustand Store With Devtools

```typescript
// file name: test.tsx
import { create } from 'zustand';
import { devtools } from 'zustand/middleware';

type State = {};

type Actions = {
  reset: () => void;
};

const initialState: State = {};

const test = create(
  devtools<State & Actions>((set) => ({
    ...initialState,
    reset: () => set(initialState),
  })),
);

export default test;
```

### ornp - Next.js Page

```typescript
export default function Page() {
  return <main className=""></main>;
}
```

### ornla - Next.js Layout

```typescript
interface Props {
  children: React.ReactNode;
}

export default function Layout({ children }: Props) {
  return <div>{children}</div>;
}
```

### ornlo - Next.js Loading

```typescript
export default function Loading() {
  return <div className=""></div>;
}
```

### orne - Next.js Error

```typescript
'use client';

interface Props {
  error: Error & { digest?: string };
  reset: () => void;
}

export default function Error({ error, reset }: Props) {
  return (
    <div className="">
      Error: {error.message}
      <button onClick={() => reset()}>Try again</button>
    </div>
  );
}
```

### ornnf - Next.js Not Found

```typescript
export default function NotFound() {
  return <div className=""></div>;
}
```

### orbc - Basic Component

```typescript
// file name: test.tsx
export default function test() {
  return <div className=""></div>;
}
```
