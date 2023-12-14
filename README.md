#  Pipeline de Integração e Entrega contínua no Jenkins

> [!IMPORTANT]
> ## Permissões 

Em primeiro momento iremos dar permissões para que possa evitar possíveis problemas de instalação. Seguindo o passo a passo:

> #### Entrar no Diretório:

```bash
  cd var/run
```

> #### Após entrar no diretório, verificar se o arquivo "docker.sock" está com as permissões necessárias:

```bash
  ls -la | grep docker.sock
```

> #### Caso as permissões não estejam concedidas. Habilitá-las utilizando o seguindo comando:

`*Obs: Não utilizar esse comando para ambientes de produção

```bash
  sudo chmod 777 docker.sock
```

> #### Verificar usuários cadastros no sistema:


```bash
  sudo chmod 777 docker.sock
```

## Criação da Pipeline:

<p align="center">
    <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/422df72c-f116-4643-9c9e-87571801c550" width="300" hspace="20"/>
    <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/25b5bea6-274c-43f0-b6fc-8f904cf23df6" width="300" hspace="20"/> 
    <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/e4e8a5eb-a9e6-471b-ac79-bf719d98f485" width="300" hspace="20"/> 
    <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/7569cdaf-66a4-4964-b60d-c5efeef30b16" width="300" hspace="20"/>
    <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/73fe9e71-a6c5-4803-b86f-0b808c64a787" width="300" hspace="20"/>
    <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/59b1f06a-479f-4362-92d8-4127d8f8a82c" width="300" hspace="20"/>
    <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/3684546e-f7c4-43e2-b20d-8394ed30a54e" width="300" hspace="20"/>
    <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/af44b0b2-4d02-4818-be3b-120d0778d1ee" width="300" hspace="20"/>
</p>
