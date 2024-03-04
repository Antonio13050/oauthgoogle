# Projeto Spring com Autenticação do Google

Este é um projeto simples em Spring que demonstra como configurar a autenticação do Google em uma aplicação web.

## Configuração

1. Clone este repositório:

```bash
git clone https://github.com/seu-usuario/seu-projeto.git
````

2. Configure as credenciais do OAuth 2.0 no Console de Desenvolvedores do Google:

- Acesse [Console de Desenvolvedores do Google](https://console.developers.google.com/)
- Crie um novo projeto ou selecione um projeto existente
- Vá para "Credenciais" no menu lateral
- Crie uma nova credencial do tipo "OAuth 2.0 Client ID"
- Adicione as URLs de redirecionamento autorizadas (por exemplo, `http://localhost:8080/login/oauth2/code/google`)
- Faça o download do arquivo JSON com as credenciais e salve-o no diretório `src/main/resources`

3. Configure as credenciais no arquivo `application.properties`:
```bash
spring.security.oauth2.client.registration.google.client-id=YOUR_CLIENT_ID
spring.security.oauth2.client.registration.google.client-secret=YOUR_CLIENT_SECRET
````

## Execução

Para executar o projeto, você pode usar o Maven. Acesse o diretório raiz do projeto e execute o seguinte comando:

```bash
mvn spring-boot:run
````
