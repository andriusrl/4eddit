![4eddit](https://i.imgur.com/UBBagOd.png)

> Status do Projeto: Em desenvolvimento :warning:

### Link de acesso
### 4eddit-andrius.surge.sh

# 4eddit

#### Implementação do front-end de uma rede real com cadastro, login, posts, likes e comentários.
<h6></h6>

### Página de login

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c10d6996-4e20-45e8-a4aa-c1d7e4710fea/Untitled.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fc10d6996-4e20-45e8-a4aa-c1d7e4710fea%2FUntitled.png?table=block&id=9df64902-45f4-4dfb-a48d-3cba6807226c&width=1060&cache=v2)

A página de login possui dois campos de texto: email e senha. O comportamento será o mesmo da página de login feita semana passada. Ao fazer o login, o usuário deverá ser redirecionado para a página de feed.

A página possui também um botão "Cadastrar", que leva o usuário para a página de cadastro.

### Página de cadastro

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/74892eaa-2276-42fc-8a0d-7ad3295f413c/Untitled.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F74892eaa-2276-42fc-8a0d-7ad3295f413c%2FUntitled.png?table=block&id=d86ff58a-1b45-4689-b41d-0addade2ea32&width=1060&cache=v2)

A página de cadastro possui 3 campos: nome de usuário, email e senha. O endpoint de cadastro retornará as mesmas informações do endpoint de login. Portanto, após cadastrar, o usuário deverá ser redirecionado para a página de feed, já estando logado (ou seja, com o token salvo no LocalStorage).

### Página de feed (lista de posts)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ae9a5889-1b48-4fc2-a9ca-bd32b632eab8/Untitled.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fae9a5889-1b48-4fc2-a9ca-bd32b632eab8%2FUntitled.png?table=block&id=d08c5c7e-e815-4fa0-a543-b9084c7e12b6&width=1060&cache=v2)

A página de feed deverá mostrar todos os posts, além de um formulário para a criação de post. O formulário possui apenas o campo de texto. Cada post mostrará o nome de usuário que postou, o texto do post, o número de votos (positivo ou negativo) e o número de comentários. Caso o usuário tenha votado positiva ou negativamente, isso deverá estar indicado. Todas essa informações serão fornecidas pela API.

Quando o usuário clicar em um post, ele deverá ser redirecionado para a página do respectivo post. 

Quando um usuário clicar em votar (positiva ou negativamente), uma requisição deverá ser feita indicando a "direção" do voto. Um voto positivo é indicado com o número `1`. Um voto negativo é indicado com o número `-1`. Para remover um voto, a direção deve ser `0`.

Essa página só pode ser acessada por um usuário logado. Caso o usuário não esteja logado, deverá ser redirecionado para a página de login.

### Página de post

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/38b78c1b-6bb4-4fb7-844b-991ed9f199da/Untitled.png](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F38b78c1b-6bb4-4fb7-844b-991ed9f199da%2FUntitled.png?table=block&id=a53989da-b39d-4d7d-b433-db99e4b390ee&width=1060&cache=v2)

A página de um post mostrará o mesmo card de post da página de feed, com o usuário, texto, curtidas e número de comentários. Abaixo, terá um formulário para criação de comentários e os cards de comentários. A estrutura é muito similar à do post, mas comentários não possuem outros comentários dentro deles. A lógica de votos é a mesma do post.

Essa página só pode ser acessada por um usuário logado. Caso o usuário não esteja logado, deverá ser redirecionado para a página de login.

# Linguagens de programação e bibliotecas utilizadas

### - JavaScript
### - ReactJS
### - React-Routes
### - MaterialUI

# Como iniciar o projeto

### Entre no diretório do projeto e execute:

### `npm install`

Instala as dependencias do projeto.

### `npm start`

Executa o aplicativo no modo de desenvolvimento.<br />
Abra [http://localhost:3000](http://localhost:3000) para visualizá-lo no navegador.

A página será recarregada se você fizer edições. <br />
Você também verá erros no console.

### `npm run build`

Cria o aplicativo para produção na pasta `build`. <br />
Ele agrupa corretamente o React no modo de produção e otimiza a construção para o melhor desempenho.

A compilação é minificada e os nomes de arquivos incluem os hashes. <br />
Seu aplicativo está pronto para ser implantado!

