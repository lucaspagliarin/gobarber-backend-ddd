
[Home](https://github.com/lucaspagliarin/gobarber-backend)

**Create User**
----
  Creates a new user and return it in json format.

* **URL**

  /users

* **Method:**

  `POST`

*  **URL Params**

    None

* **Data Params**

  ```json
    {
      "name": "string",
      "email": "string",
      "password": "string"
    }
  ```

* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
    ```json
      {
        "name": "Lucas Pagliarin",
        "email": "sample@example.com",
        "id": "6cef3728-f48c-45e4-ab85-c63bbf1caeb3",
        "created_at": "2020-04-18T20:57:29.504Z",
        "updated_at": "2020-04-18T20:57:29.504Z"
      }
    ```

* **Error Response:**

* **Sample Call:**

  ```javascript
    const response = await axios.post('/users', {
      name: "Lucas Pagliarin",
      email: "lucas.pagliarin@gmail.com",
      password: "123456"
    });
  ```
