# go-rsp
Standard response format for golang

RspBaseData:
```
{
  message: {
    message: "",
    type: ""
  },
  code: 0,
  data: null
}
```

RspPagData:
```
{
  message: {
    message: "",
    type: ""
  },
  code: 0,
  data: null,
  paginate: {
    current_page: 0,
    total_pages: 0,
    total_count: 0,
    per_page: 0
  }
}
```

default code:

```
OK = 0

// authorization
StatusUnauthorized = 10001
StatusTokenExpired = 10002
StatusInvalidToken = 10003

// users
StatusUserNotFound  = 20001
StatusErrorPassword = 20002

// crud
StatusCreateFailed       = 30001
StatusUpdateFailed       = 30002
StatusDestroyFailed      = 30003
StatusBatchCreateFailed  = 30004
StatusBatchUpdateFailed  = 30005
StatusBatchDestroyFailed = 30006
```