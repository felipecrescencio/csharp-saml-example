# csharp-saml-example

Exemplo de Aplicação DotNet Core com autenticação no IDM TOTVS Fluig Identity.  

## Créditos

Código fonte baseado no post [How to Authenticate with SAML in ASP.NET Core and C#](https://developer.okta.com/blog/2020/10/23/how-to-authenticate-with-saml-in-aspnet-core-and-csharp).  

### Configurações

As configurações do aplicativo SAML estão no arquivo `appsettings.json` seção `Saml2`.

Você deve configurar apenas UMA das opções abaixo:

#### IdPMetadata
URL do XML com as configurações do aplicativo SAML
```
"IdPMetadata": "{IDP MetaData URL}"
```
#### IdPMetadataFile
Arquivo XML com as configurações do aplicativo SAML
```
"IdPMetadataFile": "{IDP MetaData File}"
```

E finalizar com a troca da configuração nas linhas 45 e 46 do `Startup.cs`.  
