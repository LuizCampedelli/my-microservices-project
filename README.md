### Execução:

1. **Construir e iniciar os contêineres**:
No diretório raiz (`/my-microservices-project`), rode o comando:

```
docker-compose up --build
```
![host 5001](https://github.com/user-attachments/assets/bc67c159-614c-4f7f-a2ec-e2f6abbd1e21)


2. **Acessar o serviço**:
    - O app principal estará disponível em `http://localhost:5000`.
    - Para fazer uma requisição ao app com validação de token, você pode usar `curl` ou outra ferramenta, por exemplo:

```
curl -H "Authorization: valid-token" http://localhost:5001/validate
```

![validacao](https://github.com/user-attachments/assets/3a087f29-ba39-46d3-b604-963f54d8a283)

Se vc estiver no powershell:

```
Invoke-WebRequest -Uri "http://localhost:5001/validate" -Headers @{ Authorization = "valid-token" }
```


### Divirta-se
