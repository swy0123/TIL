Next.js & React - 완벽 정복 가이드 (incl. Two Paths!)
## Section 1. 시작하기

### Nextjs 이점
1. Fullstack Apps
2. File-based Routing
3. Server-side Rendering

### 첫번째 앱 생성
- npx create-next-app@latest</br>
![image](https://github.com/swy0123/TIL/assets/61828877/852b31d6-3398-4c50-9ffe-dcb27db153cc)
- npm run dev

### 첫번째 앱 편집
https://codesandbox.io/p/devbox/nextjs-basic-app-k2yfy7

<hr>

## 에러 정리

#### 파일 경로에 "/ude" 들어가면 안됨
![image](https://github.com/swy0123/TIL/assets/61828877/c24c9506-086e-4283-9a7e-91eb8d4f0015)

https://stackoverflow.com/questions/77278303/next-js-13-error-byte-index-out-of-bounds-on-npm-run-dev
으로 해결

#### babel 모듈 및 EsLint 에러
현재 프로젝트 폴더의 상위 폴더로 프로젝트를 열면 발생하는 문제<br>
babelrc 등의 설정으로 해결할 수 있으나 <br>
https://stackoverflow.com/questions/68163385/parsing-error-cannot-find-module-next-babel/68838570#68838570 으로 해결
