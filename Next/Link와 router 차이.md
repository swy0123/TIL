## Link와 router(useRouter) 차이
### Link
Next.js의 Link태그는 Next.js에서 제공하는 컴포넌트 중 하나
next 13 버전 이후로부터는 Link 태그 속에 a 태그 넣지 않아야 정상 작동
#### href
href props는 Link태그를 사용할 때 필수로 사용 
- 사용자 경험적인 측면과 SEO적인 측면
- href가 없다면 새 창으로 보기 (ctrl + click)이 작동하지 않음
- href가 없다면 검색엔진이 추적을 할 수 없음
#### replace
replace props는 기본값이 false
replace가 존재한다면 browser history에 현재 기록상태를 대체
#### prefetch
prefetch props가 존재한다면 href주소를 미리 읽어와 해당 페이지의 리소스들을 미리 받음

<hr>

### useRouter
useRouter는 next.js에서 함수형식으로 routing을 해주는 라이브러리
- router.push(href) : href로 탐색을 실행하고, browser history에 쌓음
- router.replace(href) : href로 탐색을 실행하지만 browser history에 쌓지는 않음
- router.refresh(): 현재의 경로를 새로고침. 서버에서 새로운 요청을 만들고, 구성요소들을 재렌더링
- router.prefetch(href) : href를 prefetching
- router.back() : browser history에서 이전 경로로 이동
- router.forward() : browser history에서 다음 페이지로 이동

<hr>
Next.js에서는 특별한 이유가 없다면 Link를 사용하는 것을 추천
