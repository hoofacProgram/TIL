# Devexpress
>출처 : [Devexpress](https://www.devexpress.com)

## DataGrid
- 해당 화면의 column 순번 입력할 때 사용한다.
```javascript
cellTemplate: function(cellElement, cellInfo) { cellElement.text(cellInfo.row.rowIndex) } }
```

- 컬럼에 링크 태그 추가.
```
{ dataField: 'doc_no', caption: '문서번호', width: '12%', alignment: 'center', allowEditing: false,
    cellTemplate: function (container, options) {
      $('<a>' + options.text + '</a>')
      .attr('href' , doc_url + options.value)
      .attr('target', '_blank')
      .appendTo(container);
    }
  }
```

- 특정 행의 셀값을 가져올 때 사용한다.
```javascript
// 0번 행의 'nm' 컬럼의 내용을 가져온다.
$('#main-grd').dxDataGrid("instance").cellValue(0, 'nm')
```

- grid의 checkBox의 선택을 취소시킨다.
```
const selectRow = e.component.getSelectedRowKeys();
e.component.deselectRows(selectRow);
```

### Option
- onInitNewRow : 내용 추가 row가 생성될때.
  - 생성된 row 삭제
  ```
  e.component.refresh(true).done(() => {
    e.component.cancelEditData();
  });
  ```

- onContentReady : grid가 완전히 그려지고 난 이후.

- onCellClick : grid 내부의 cell을 클릭했을 때.

- onSaving : grid 추가 row의 내용이 저장될 때.

### Attribute
### allowEditing: false
- 특정 셀을 readOnly로 만든다.
```javascript
, { dataField: 'nm', caption: '성명', width: '9%', alignment: 'center', allowEditing: false }
```

## Button
- 버튼 속성 설정에 사용한다.
```javascript
$('.save-btn').dxButton({ disabled: true })
```