---
layout: default
comments: true
# other options
---
## Creazione del blog in Github Pages con Jekyll

Prima di tutto ho seguito la guida github, creato il repository [http://vDallAcqua.github.io](http://vDallAcqua.github.io) e questo diventerà il sito vero e proprio del blog.
Il branch master è quello che viene usato per la pubblicazione.

Per installare un tema di pages devo installare in locale jekyll. Per questo ho, via chocolatey che è veramente bello e nuovo, fatto da cmd prompt (amministrativo):

```shell_session
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
choco install ruby -y
```

Download di rubygems aggiornato e anche il certificato da copiare nella installazione di rubygems da [qui](http://guides.rubygems.org/ssl-certificate-update/#installing-using-update-packages), prompt comandi:

```shell_session
gem install --local rubygems-update-2.6.7.gem
gem uninstall rubygems-update
gem install bundler
```


Come tema ho scelto il [beautiful Jekyll](https://github.com/daattali/beautiful-jekyll#readme) fra i tanti. Ho seguito le istruzioni del readme, che essenzialmente ti dicono di prendere tutti i files del tema e copiarli pari pari sul tuo sito pages. Il modo più semplice di farlo è fare un fork del progetto originale su github al link precedente. Ci si trova con un sito che è una replica esatta del tema e che poi in modo abbastanza veloce si può adattare alle proprie esigenze.

Ho fatto anche il primo `bundle update` anche perchè il "Gemfile" mi include la gem `paginate`. Si è installata con l'update per cui funziona proprio tutto.
Adesso qualche sistemazione ulteriore, tipo l'aggiunta dei commenti disqus ecc. ed è fatto. 

E quindi: Hello World!
