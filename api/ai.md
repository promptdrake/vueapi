---
outline: deep
---
# Ai Request
Lakukan Request Kedalam Ai
<br>
*Ai Yang Tersedia Didalam Bot*
| Name        |      Endpoint      |  Parameter |
| ------------- | :-----------: | ----: |
| Bard      | /api/v1/ai/bard | apikey, text |
| Translate      | /api/v1/ai/translate | apikey, text, to |
| Simi      | /api/v1/ai/simi | apikey, text |
| Tts     | /api/v1/ai/tts | apikey, text |
| Tts     | /api/v1/ai/nulis | apikey, text |
| Midjourney     | /api/v1/ai/midjourney | apikey, text |
| Cartoon Ai     | /api/v1/ai/cartoonai | apikey, text |
| Gpt 3    |   /api/v1/ai/gpt    |   apikey, text |
| Gpt 4    |   /api/v1/ai/gpt4    |   apikey, text |
| Blackbox    |   /api/v1/ai/gpt4    |   apikey, text, webSearchMode  |

## Example Response (200)

- Simsimi Api
```json
{
  "status": true,
  "code": 200,
  "author": "Aisbir Dev",
  "result": {
    "question": "hai",
    "answer": "Apasih so asik lo"
  }
}
```

- Chatgpt 3, 4, bard
```json
{
  "status": true,
  "author": "Aisbir Dev",
  "code": 200,
  "result": "Hello! It looks like you're referencing the video game series \"Halo.\" What would you like to know or discuss about Halo?"
}
```

- Midjourney, cartoonai
```json
{
  "status": true,
  "author": "Aisbir Dev",
  "code": 200,
  "result": "https://loyisa.aisbircubes.my.id/api/storage?file=1716698914673.jpg"
}
```

- Translate
```json
{
  "status": true,
  "author": "Aisbir Dev",
  "code": 200,
  "to": "id",
  "result": "Hai"
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