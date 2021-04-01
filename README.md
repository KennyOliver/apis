# apis

![CodeFactor](https://www.codefactor.io/repository/github/KennyOliver/apis/badge?style=for-the-badge)
![Latest SemVer](https://img.shields.io/github/v/tag/KennyOliver/apis?label=version&sort=semver&style=for-the-badge)
![Repo Size](https://img.shields.io/github/repo-size/KennyOliver/apis?style=for-the-badge)
![Total Lines](https://img.shields.io/tokei/lines/github/KennyOliver/apis?style=for-the-badge)

**Self-hosted static REST APIs**

[![repl](https://replit.com/badge/github/KennyOliver/kennyolivergithubioapis)](https://replit.com/@KennyOliver/kennyolivergithubioapis)

## Testing
JAVASCRIPT
```javascript
const url = "https://kennyoliver.github.io/apis/testing/fake-user-data.json";

function getUserData(URL) {
  fetch(URL)
    .then(res => res.json())
    .then(data => {
      //json vaiable contains object with data
      console.log(data);
      console.log(data[0].id);
      
      console.log("All usernames:");
      for (let i = 0; i < data.length; i++) {
        console.log(data[i].username);
      }
    });
}

getUserData(url);
```

PYTHON
```python
import requests
response = requests.get("https://kennyoliver.github.io/apis/testing/fake-user-data.json")
print(response.status_code)
data = response.json()
print(data)
print(data[0])
print(data[0]["id"])
print(data[0]["first_name"])
print(data[0]["last_name"])
print(data[0]["email"])
print(data[0]["username"])
```

---
Kenny Oliver ©2021
