
[Home](https://github.com/lucaspagliarin/gobarber-backend)

**Create User**
----
  Add a new avatar to the authenticated user and returns the user in json format.

* **URL**

  /users/avatar

* **Method:**

  `PATCH`

*  **URL Params**

    None

* **Data Params**

  Multipart form: 'avatar' file

* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
    ```json
      {
        "id": "6cef3728-f48c-45e4-ab85-c63bbf1caeb3",
        "name": "Lucas Pagliarin",
        "email": "lucas.pagliarin@gmail.com",
        "avatar": "b0fd0016a78f6b8fec54-35429320_309587776247614_3249685037699825664_n.jpg",
        "created_at": "2020-04-18T20:57:29.504Z",
        "updated_at": "2020-04-25T22:03:41.844Z"
      }
    ```

* **Error Response:**

* **Sample Call:**

  ```javascript

  ```
