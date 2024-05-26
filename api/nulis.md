---
outline: deep
---

# Nulis Rest Api
Membuat Tulisan di kertas<br>
Parameter:
`/api/v1/fun/nulis`

## Example Response 200
```json
{
    "status": true,
    "author": "Aisbir Dev",
    "result":"https://loyisa.aisbircubes.my.id"
}
```

## Example Response (401, 500, 402)
```json
{
  "status": false,
  "code": 401,
  "author": "Aisbir Dev",
  "data": "apikey.notfound.exception.key",
  "message": "Api ini Sudah Limit, Silahkan Purchase untuk mendapatkan unlimited ip"
}
```