## Handshake

**Translations**

- [EN-US](./handshake.md)
- [PT-BR](./pt_br/handshake.md)

## Navigation
<details>
<summary><b>Menu</b></summary>

- [What is a Handshake](#what-is-a-handshake)
- [Handshake Methods](#handshake-methods)
- [Credits](#credits)
</details>

<br />

# What is a Handshake
- What is a Handshake
  - It is when requests (methods) are sent or received in a system or application.

<br /><br />
<center>
	<img width="600" src="./assets/how_it_works_handshake.png">
</center>
<br /><br />

# Handshake Methods

- **GET**: Using `GET` you request data from a resource (server);
  - Returns key and value in the URL;
  - Best used when working with APIs.
- **POST**: Using `POST` you can send data to the server, create/update a resource;
  - Does not return key and value in the URL;
  - Best used for forms with information that must remain private.

**Examples**:

**GET** https://mywebsite.com/page?key=value

**POST**: http://mywebsite.com/page

- Client: User;
- Server: Server (Data Center).
<center>
	<img width="650" src="./assets/get_vs_post_and_payload.png" />
</center>
<br />

- **HEAD**: It is the `GET` method that does not return anything in the body of the webpage.
- **PUT**: It is the `POST` method that does not perform a full handshake if the sent information is the same.
<br />
<br />

<br />

# Credits

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
