# Devexpress
>[Devexpress](https://www.devexpress.com)

## DataGrid
- 컬럼에 버튼 추가
```javascript
  , { name: 'openBtn', caption: 'I/F', type: 'buttons', width: '25%',
      // text 대신 icon 사용 가능(혼용은 안됨)
      buttons: [ { text: '[실행]', onClick: (e) => {
        //함수 실행
      } } ] }
```
- 해당 화면의 column 순번 입력할 때 사용한다.
```javascript
// 그리드 컬럼 자체 생성
cellTemplate: function(cellElement, cellInfo) { cellElement.text(cellInfo.row.rowIndex) }
```
```javascript
// 그리드 옵션에서 처리
column : { dataField: 'seq', width: '5%', caption: '순번', alignment: 'center'}
g.option.onCellPrepared = (e) => {
    if (e.rowType === 'data' && e.columnIndex === 0) {e.data.seq = e.rowIndex + 1; e.cellElement.text(e.data.seq);}
}
```

- 컬럼에 링크 태그 추가.
```javascript
{ dataField: 'doc_no', caption: '문서번호', width: '12%', alignment: 'center', allowEditing: false,
    cellTemplate: function (container, options) {
      $('<a>' + options.text + '</a>')
      .attr('href' , doc_url + options.value)
      .attr('target', '_blank')
      .appendTo(container);
    }
  }
```

- 컬럼에 데이터 입력한다.
```javascript
// grid 내부
setCellValue(rowData, value) { rowData.board_gb = value; },
// grid 외부 : mainGrid에 Id 넣고 ColumnName 넣고, data 넣는다.
mainGrid.dataGrid.cellValue(Id, 'ColumnName', 'data')
```

- grid의 instance 정보를 사용할 수 있다.
```javascript
const gridData = $('#grid').dxDataGrid('instance');
```

- grid의 선택한 row의 정보를 사용할 수 있다.
```javascript
const selectedRowData = $('#grid').dxDataGrid('instance').getSelectedRowsData();
```

- grid의 dataSource를 가져온다.
```javascript
const dataSource = $('#grid').dxDataGrid('instance').option('dataSource');
const firstRow = dataSource[0]; // 인덱스 '0' row data
```

- 특정 행의 셀값을 가져올 때 사용한다.
```javascript
// 0번 행의 'nm' 컬럼의 내용을 가져온다.
$('#main-grd').dxDataGrid("instance").cellValue(0, 'nm')
```

- grid의 checkBox의 선택을 취소시킨다.
```javascript
const selectRow = e.component.getSelectedRowKeys();
e.component.deselectRows(selectRow);
```

### Option
- onInitNewRow : 내용 추가 row가 생성될때.
  - 생성된 row 삭제
  ```javascript
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