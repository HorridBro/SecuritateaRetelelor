# SecuritateaRetelelor

In acest laborator vom rezolva un exercitiu de tip CTF pe tema de securitate web.

## Pasul 1
#### Instalati docker https://docs.docker.com/install/linux/docker-ce/ubuntu/
#### Luati imaginea de docker pentru a rezolva acest laborator
```
sudo docker pull mihneass/websecurity
```
#### Porniti imaginea
```
sudo docker run -d -p 80:80 mihneass/websecurity
```

## Pasul 2
La pasul 1 am pornit o imagine cu un web server Apache care foloseste o versiune veche de PHP.

Pentru a rezolva acest laborator trebuie sa gasiti cheia care se afla in fisierul cu calea: **/etc/secret** prezent in containerul pe care l-am pornit la pasul 1.

Acest exercitiu poate fi rezolvat doar cu ajutorul browserului, accesand urmatorul [link](http://localhost)

Indicii:
* Serverul Apache este configurat default
