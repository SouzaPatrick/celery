## python version 3.10

Adicionar flacke8 ao projeto
sudo apt install flake8

Dentro da pasta do projeto insira os comandos
flake8 --install-hook git
git config flake8.strict true

Iniciar RabbitMQ pelo docker
```
> docker run -d -p 5672:5672 rabbitmq
```

Iniciar o worker do celery
```
celery -A tasks worker -l info
```

Iniciar o dashboard, flower
```
celery -A tasks flower
```

Executar o codigo
```
python app.py
```