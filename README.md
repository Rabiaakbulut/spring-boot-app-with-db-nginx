# Docker Compose - CRUD API - NGINX Reverse Proxy

![chart2](https://user-images.githubusercontent.com/47069895/53306460-40c57900-3885-11e9-88e5-d2b94b4a4003.jpg)

## Uygulama Hakkında
* Bu uygulamada CRUD API'ler ile not tutabiliriz. 
* Veri tabanı olarak MySQL kullanılmış. 
* Reverse proxy olarak NGINX kullanılmış.

## Uygulamanın Çalıştırılması 

* Uygulamayı klonlama

```
git clone https://github.com/Rabiaakbulut/spring-boot-app-with-db-nginx.git
```

* Uygulamayı çalıştırma

```
> docker-compose up -d
```

* Uygulamayı görmek için: http://localhost:7070

![localhost](/img/localhost.png)


## Postman CRUD Testi

* POST /api/notes
![post](/img/post.png)

* GET /api/notes , /api/notes/{noteId}
![get](/img/get.png)
<img src="get.jpg" alt="get" style="width:200px;"/>

* PUT /api/notes/{noteId}
![put](/img/put.png)

* DELETE /api/notes/{noteId}
![delete](/img/delete.png)
