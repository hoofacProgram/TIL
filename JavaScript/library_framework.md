lodash
- 배열 등의 정렬이나 정리

Moment.js
- 날짜, 시간
- 참고
  - https://jsikim1.tistory.com/195

```javascript
// 오늘 날짜 포멧에 맞춰서 입력
moment().format('YYYY-MM-DD');
// 날짜 및 시간 더하기
moment().add(1, "y").format();  // '1' 년 더하기
moment().add(1, "M").format();  // '1' 월 더하기
moment().add(1, "w").format();  // '1' 주 더하기
moment().add(1, "d").format();  // '1' 일 더하기
moment().add(1, "h").format();  // '1' 시 더하기
moment().add(1, "m").format();  // '1' 분 더하기
moment().add(1, "s").format();  // '1' 초 더하기
// 날짜 및 시간 빼기
moment().subtract(1, "y").format();  // '1' 년 빼기
moment().subtract(1, "M").format();  // '1' 월 빼기
moment().subtract(1, "w").format();  // '1' 주 빼기
moment().subtract(1, "d").format();  // '1' 일 빼기
moment().subtract(1, "h").format();  // '1' 시 빼기
moment().subtract(1, "m").format();  // '1' 분 빼기
moment().subtract(1, "s").format();  // '1' 초 빼기
```

Luxon
- 시간 관련

handsontable
- 엑셀 형태의 스프레드시트 만들기

D3
- 데이터 시작화

chart.js
- 차트, 그래프

three.js
- 3D 삼차원 그래픽

jsdoc
- 주석, 문서화 (원조격은 Java의 Javadoc)