# SecuritateaRetelelor

In acest laborator vom rezolva un exercitiu de tip CTF de securitate web.

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
La pasul 1 am pornit o imagine de Ubuntu care contine un web server Apache.

Pentru a rezolva acest laborator trebuie sa gasiti cheia care se afla in fisierul cu calea: **/etc/secret** prezent in containerul pe care l-am pornit la pasul 1.

Acest exercitiu poate fi rezolvat doar cu ajutorul browserului, accesand urmatorul [link](http://localhost)

Indicii:
* Serverul Apache are o configuratie default, deci locatia scripturilor care ruleaza pe web server e cunoscuta. 
* Ar trebui sa va uitati la url si sa observati cum se schimba cand accesati link-ul precizat mai sus. 
* Versiunea de PHP folosita este foarte veche si poate permite multe exploit-uri.

Daca ati ajuns la o pagina cu mai multe mesaje in engleza, puteti cauta accesa urmatorul [link]http://www.google.com/search?q=php+null+byte+injection
