## Creazione blog in pages

Prima di tutto ho seguito la guida github, creato il repository http://vDallAcqua.github.io e questo diventerà il sito vero e proprio del blog.
Il branch master è quello che viene usato per la pubblicazione.

Per installare un tema di pages devo installare in locale jekyll. Per questo ho, via chocolatey che è veramente bello e nuovo, fatto da cmd prompt (amministrativo):

'''
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
choco install ruby -y
'''

Download di rubygems aggiornato e anche il certificato da copiare nella installazione di rubygems da http://guides.rubygems.org/ssl-certificate-update/#installing-using-update-packages, prompt comandi:

'''
gem install --local rubygems-update-2.6.7.gem
gem uninstall rubygems-update
gem install bundler
'''

Ho fatto anche il primo 'bundle update' anche perchè il "Gemfile" mi include la gem 'paginate'. Si è installata per cui funziona proprio tutto.
Adesso qualche sistemazione ulteriore, tipo l'aggiunta dei commenti disqus ecc. ed è fatto. 




