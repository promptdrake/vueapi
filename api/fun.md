---
outline: deep
---
# Image Maker Funi
Api disini berfungsi untuk generate Image
<br>
*Maker Yang Tersedia Didalam Bot*
| Name        |      Endpoint      |  Parameter |
| ------------- | :-----------: | ----: |
| Welcomer     | /api/v1/fun/welcomer | apikey, background, text1, text2, text3, avatar |
| imagequote     | /api/v1/fun/imagequote | apikey, image, text, author |
| hue     | /api/v1/fun/hue | apikey, image, deg |
| nokia     | /api/v1/fun/nokia | apikey, image |
| adios     | /api/v1/fun/adios | apikey, image |
| jail     | /api/v1/fun/jail | apikey, image |
| communism     | /api/v1/fun/communism | apikey, image |
| wanted     | /api/v1/fun/wanted | apikey, image |
| drip     | /api/v1/fun/drip | apikey, image |
| invert     | /api/v1/fun/invert | apikey, image |
| greyscale     | /api/v1/fun/greyscale | apikey, image |
| supreme     | /api/v1/fun/supreme | apikey, text |
| sadcat     | /api/v1/fun/sadcat | apikey, text |
| blur     | /api/v1/fun/blur | apikey, image |

## Example Response (200)
Response:<br> 
image/jpeg<br>

Jadi Kalian bisa langsung throw result
soalnya result api ini udh format jpg / png

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