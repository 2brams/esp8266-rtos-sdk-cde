<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/Ey1Hllw.jpg" alt="Project logo"></a>
</p>

<h3 align="center">ESP8266 RTOS SDK Common Development Environment (CDE)</h3>

---

<p align="center"> Automatisation de l'installation du SDK ESP8266 RTOS de Espressif disponible  <a href="https://docs.espressif.com/projects/esp8266-rtos-sdk/en/latest/get-started/index.html#get-esp8266-rtos-sdk" rel="">ici</a> en IaC.
<br> 
</p>


## 📝 Table of Contents

- [About](#about)
- [Usage](#usage)
- [What now?](#now)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)

## 🧐 About <a name = "about"></a>

Ce projet permet de créer un CDE Docker et d'automatiser la configuration de l'environnement logiciel pour le développement d'applications utilisant du matériel basé sur l'Espressif ESP8266EX.

## Prerequisites

Pour utiliser ce dépôt, vous devez installer Packer, Ansible et Docker sur votre machine. Les versions de chaque outil utilisé pour ce dépôt sont:

```
Packer: 1.7.2
Ansible: 2.9.20
Docker: 20.10.6
```

## 🎈 Usage <a name="usage"></a>

Pour créer l'image docker.

```
packer build esp8266-cde-docker.json
```
Pour pouvoir flasher le matériel depuis le container Docker il faut utiliser le paramètre "device".

```
docker run -ti --device=/dev/ttyUSB0 image:version -c bash
```


## 🔗 What now? <a name = "now"></a>

Allez sur le [Guide](https://docs.espressif.com/projects/esp8266-rtos-sdk/en/latest/get-started/index.html#get-esp8266-rtos-sdk) de programmation ESP8266 RTOS SDK pour développer vos applications.

## ✍️ Authors <a name = "authors"></a>

- [@2brams](https://github.com/2brams) - Idea & Initial work


## 🎉 Acknowledgements <a name = "acknowledgement"></a>

- [@dimtass](https://bitbucket.org/dimtass) - Inspiration

