---
outline: deep
---
# Upload Request

Untuk Mengirim Request Upload File Gunakan kode seperti dibawah<br>
Proses Upload Tidak Memerlukan Parameter Apikey
```js
/*
* Dev: Promptdrake
* instagram: aisbircubess
* github: github.com/promptdrake
* Base Uri: On Get Started Page
*/
async function aisbirCdn(filePath) {
  const formData = new FormData();
  formData.append('file', fs.createReadStream(filePath));

  try {
    const response = await fetch("/api/v1/upload", {
      method: 'POST',
      body: formData
    });

    if (response.ok) {
      const fileUrl = await response.json();
      return fileUrl
    } else {
      const errorResponse = await response.json();
      return false
    }
  } catch (error) {
   return false
  }
}

// Example usage:
aisbirCdn(filePath);
aisbirCdn('./database/list.json');
```
