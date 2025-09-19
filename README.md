# README

```bash
source .venv/bin/activate
```

Il suffit ensuite de lancer le jupyter-book:
```bash
cd book
jupyter book start
```

Pour accéder à l'URL depuis windows : 
```bash
ip addr show eth0
```

Puis prendre l'adresse ip devant `inet` (ex: `inet 172.31.208.202/20 brd 172.31.223.255 scope global eth0`), et accéder à : `http://172.31.208.202:3000/`

Pour permettre un export en PDF, voici les librairies à installer dans l'environnement venv.
```bash
sudo apt update
sudo apt install -y \
  texlive-xetex \
  texlive-latex-recommended \
  texlive-latex-extra \
  texlive-fonts-recommended \
  texlive-fonts-extra \
  latexmk
```