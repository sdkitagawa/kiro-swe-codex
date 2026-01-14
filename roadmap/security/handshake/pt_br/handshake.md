## Handshake

**Translations**

- [EN-US](../handshake.md)
- [PT-BR](./handshake.md)

## Navigation
<details>
<summary><b>Menu</b></summary>

- [O que é o Handshake](#o-que-é-o-handshake)
- [Métodos de Handshake](#métodos-de-handshake)
- [Credits](#credits)
</details>

<br />


# O que é o Handshake
- O que é o Handshake
  - É quando há envio ou recebimento de requisições (métodos) em um sistema ou aplicação.

<br /><br />
<center>
	<img width="600" src="../assets/how_it_works_handshake_pt_br.png">
</center>
<br /><br />

# Métodos de Handshake

- **GET**: Usando `GET` você faz requisição de dados de um recurso (servidor);
  - Retorna chave e valor no endereço;
  - Melhor aproveitado quando usado para APIs.
- **POST**: Usando `POST` você pode enviar dados para servidor, criar/atualizar um recurso;
  - Não retorna chave e valor no endereço;
  - Melhor usado para formulários com informações que devem permanecer privadas.

**Exemplos**:

**GET** https://meusite.com/pagina?chave=valor

**POST**: http://meusite.com/pagina

- Client: Usuário;
- Server: Servidor (Data Center).
<center>
	<img width="650" src="../assets/get_vs_post_and_payload_pt_br.png" />
</center>
<br />

- **HEAD**: Ele é o método `GET` que não retorna nada no corpo (body) da página web.
- **PUT**: Ele é o método `POST` que não efetua um novo handshake completo caso a informação enviada seja a mesma.
<br />
<br />

# Credits

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
