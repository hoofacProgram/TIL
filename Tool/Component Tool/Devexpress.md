# Devexpress
>출처 : [Devexpress](https://www.devexpress.com)

## DataGrid
- column에 순번 카운터 입력할 때 사용한다.
```javascript
cellTemplate: function(cellElement, cellInfo) { cellElement.text(cellInfo.row.rowIndex) } }
```

- 특정 행의 셀값을 가져올 때 사용한다.
```javascript
// 0번 행의 'nm' 컬럼의 내용을 가져온다.
$('#main-grd').dxDataGrid("instance").cellValue(0, 'nm')
```

## Button
- 버튼 속성 설정에 사용한다.
```javascript
$('.save-btn').dxButton({ disabled: true })
```