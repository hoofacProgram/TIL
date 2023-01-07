# CSS
## Selector

## Attr
### Dark Mode
- 운영체제(브라우저)의 설정에 따라 다크모드 설정 기능.
```css
@media (prefers-color-scheme: light) {
  /* 라이트 모드에 적용할 스타일 정의 */
  body {
    background-color: white;
    color: black;
  }
}
@media (prefers-color-scheme: dark) {
  /* 다크 모드에 적용할 스타일 정의 */
  body {
    background-color: black;
    color: white;
  }
}
```

padding 순서(시계방향?)
- top right bottom left