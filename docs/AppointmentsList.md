**List Appointments**
----
  Returns the list of all appoinments in json format.

* **URL**

  /appointments

* **Method:**

  `GET`

*  **URL Params**

    None

* **Data Params**

  None

* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
    ```json
    [
      {
        "id": "d52785dc-a002-423d-807e-b17b430b6877",
        "provider_id": "6cef3728-f48c-45e4-ab85-c63bbf1caeb3",
        "date": "2020-04-18T19:00:00.000Z",
        "created_at": "2020-04-18T22:01:22.740Z",
        "updated_at": "2020-04-18T22:01:22.740Z"
      },
    ]
    ```

* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "Invalid JWT token" }`

* **Sample Call:**

  ```javascript
    const response = await axios.get('/appointments');
  ```
