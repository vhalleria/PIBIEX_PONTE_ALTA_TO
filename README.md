# PIBIEX_PONTE_ALTA_TO

 <h3 align="center"> Software de Logística Sustentável para Alimentos e Bebidas Locais. </h3>
 
 <h4 align="center">
 O projeto visa desenvolver um software inovador destinado a atender às demandas específicas da cadeia de alimentos e bebidas no Estado do Tocantins. Este software será uma solução abrangente e integrada, projetada para otimizar todas as etapas do processo logístico.
</h4>

<p align="left">
Seguindo o MVC - Model, View, Controle (Modelo, visão e Controlador) que é um padrão de arquitetura de software que separa a informação (e as regras de negócio) da interface com a qual o usuário interage. SEGURANÇA e FACILIDADE EM MANUTENÇÃO.

O Model - Toda e qualquer ação que envolve a recuperação, atualização e remoção de dados. O Model é responsavel pela solicitação de informações, onde os dados são manipulados.

A View é responsável por manipular os dados para exibição e exibi-los. Recebe os dados, manipula e exibe os dados. (Front-end)

O controller é responsável pela comunicação entre o View e o Model. Para cada View existe um Controller especifico.

</p>


# Projeto

Links Úteis:

-   :tada: [Saiba Mais](https://linktr.ee/especializati)
-   :tada: [Curso de Larave Gratis] (https://www.youtube.com/playlist?list=PLzVtNSpnU428TMseRKw6h-2U10RnrwtmC)

## Passo a passo para rodar o projeto

Clone o projeto

```sh
git clone https://github.com/vhalleria/PIBIEX_PONTE_ALTA_TO.git PIBIEX_PONTE_ALTA_TO
```

```sh
cd PIBIEX_PONTE_ALTA_TO
```

Crie o Arquivo .env

```sh
cp .env.example .env
```

Atualize essas variáveis de ambiente no arquivo .env

```dosini
APP_NAME="PIBIEX PA"
APP_URL=http://localhost:8989

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=nome_que_desejar_db
DB_USERNAME=nome_usuario
DB_PASSWORD=senha_aqui

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
```

Suba os containers do projeto

```sh
docker-compose up -d
```

Acesse o container

```sh
docker-compose exec app bash
```

Instale as dependências do projeto

```sh
composer install
```

Gere a key do projeto Laravel

```sh
php artisan key:generate
```

Acesse o projeto
[http://localhost:8989](http://localhost:8989)
