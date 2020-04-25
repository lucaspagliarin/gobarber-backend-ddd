
[Home](https://github.com/lucaspagliarin/gobarber-backend)

**Create Session**
----
  Creates a new session and returns the user and the token in json format.

* **URL**

  /sessions

* **Method:**

  `POST`

*  **URL Params**

    None

* **Data Params**

  ```json
    {
      "email": "string",
      "password": "string",
    }
  ```

* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
    ```json
      {
        "user": {
          "id": "6cef3728-f48c-45e4-ab85-c63bbf1caeb3",
          "name": "Lucas Pagliarin",
          "email": "lucas.pagliarin@gmail.com",
          "avatar": "4c39a1f88b4eb8039f9a-35429320_309587776247614_3249685037699825664_n.jpg",
          "created_at": "2020-04-18T20:57:29.504Z",
          "updated_at": "2020-04-18T23:55:21.540Z"
        },
        "token": "token"
      }
    ```

* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "Invalid JWT token" }`

* **Sample Call:**

  ```javascript
    const response = await axios.post('/sessions', {
      email,
      password,
    });
  ```
