# pandas

```python
# read_json 기본 typ='Frame'로 되어있다.
# Series에서 사용시, typ 설정하지 않으면 불러온 데이터 제대로 사용 안된다.
pd.read_json(path, typ='series')
```