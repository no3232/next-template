## Technology

- [TypeScript](https://www.typescriptlang.org/)
- [React](https://reactjs.org/)
- [NextJS 14](https://nextjs.org/)
- [TanStack Query](https://react-query.tanstack.com/)
- [Vanilla Extract](https://vanilla-extract.style/)

## folder structure

```
📦src
 ┣ 📂apis
 ┣ 📂app
 ┣ 📂components
 ┣ 📂constants
 ┣ 📂context
 ┣ 📂hooks
 ┣ 📂lib
 ┣ 📂queries
 ┃ ┣ 📂mutation
 ┃ ┗ 📂query
 ┣ 📂stores
 ┣ 📂styles
 ┣ 📂types
 ┗ 📂utils
```

- apis: 백엔드와 통신 함수(fetch)
- app: nextjs app router, 페이지 컴포넌트
- components: 페이지에서 사용할 컴포넌트
    - 공통으로 사용할 컴포넌트는 common폴더를 생성
- constants: 고정된 상수
- context: Provider를 이용할 부분들
- hooks: 리액트 커스텀 훅
- lib: 이외 라이브러리 관련 폴더
- queries: 리액트 쿼리
    - query: useSuspensQuery
    - mutation: useMutation
- store: zustand 관련
- styles: 스타일(vanilla extract)관련 함수
- types: 타입
- utils: 모듈화 할 함수들

## Lint

- import/no-cycle: 순환 의존성(circular dependency)을 방지합니다.
- import/no-unresolved: 해석할 수 없는 import를 방지합니다.
- react/jsx-key: JSX 내에서 반복되는 엘리먼트에 key prop을 사용하지 않아도 됩니다.
- react/no-unescaped-entities: HTML 엔티티를 문자열에서 직접 사용할 수 있습니다.
- react/self-closing-comp: self-closing을 강제합니다.
- react/jsx-first-prop-new-line: 첫 번째 JSX 속성을 새로운 줄에서 시작하도록 강제합니다.
- comma-dangle: 여러 줄의 배열 및 객체 리터럴에서 항상 마지막에 쉼표를 사용합니다.
- eqeqeq: == 대신 ===를 사용하도록 권장합니다.
- indent: 들여쓰기는 2칸입니다.
- quotes: 단일 따옴표 사용을 강제합니다.
- eol-last: 파일 끝에 빈 줄을 넣습니다.
- semi: 세미콜론 사용을 강제합니다.
- simple-import-sort/imports, simple-import-sort/exports: import 및 export 문을 정렬합니다.
- jsx-quotes: JSX에서는 단일 따옴표를 사용합니다.
- no-unused-vars: 사용하지 않는 변수를 금지합니다.
- unused-imports/no-unused-imports-ts: 사용하지 않는 TypeScript import를 금지합니다.
- comma-spacing: 쉼표 뒤에 공백을 넣습니다.
- import/consistent-type-specifier-style: 항상 최상위 수준의 타입 지정 스타일을 사용합니다.
- import/newline-after-import: import 후 새 줄을 추가합니다.
- @typescript-eslint/no-unused-vars: TypeScript에서 사용하지 않는 변수에 대해 경고합니다.
- @typescript-eslint/ban-types: 일부 타입 사용을 금지합니다.
- react/display-name: React 컴포넌트의 display name을 강제하지 않습니다.
- @typescript-eslint/no-empty-function: 빈 함수를 허용합니다.

[참고 링크](https://github.com/Nexters/keyme-frontend/blob/main/.eslintrc.js)