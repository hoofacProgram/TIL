# Python

## data_type

list
dictionary

## function
map()
len()


## 스레드
- 스레드 타겟팅할때 함수명 뒤에() 붙이면 실행된다.
- 안붙이면 타겟 설정만 되고 실행은 안된다.
```
def call_websocket():
  asyncio.run(websocket_connect())

web_thread = threading.Thread(target=call_websocket)
```