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
    <figure>
        <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/422df72c-f116-4643-9c9e-87571801c550" width="400" hspace="20"/>
        <figcaption>Login no Sistema</figcaption>
    </figure>
    <figure>
        <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/25b5bea6-274c-43f0-b6fc-8f904cf23df6" width="400" hspace="20"/> 
        <figcaption>Criar Tarefa</figcaption>
    </figure>
  <figure>
        <img src="https://github.com/diegofernandesss/pipeline/assets/88402851/e4e8a5eb-a9e6-471b-ac79-bf719d98f485" width="400" hspace="20"/> 
        <figcaption>Inserir nome da Pipeline, Selecionar a Pipeline</figcaption>
    </figure>
</p>

