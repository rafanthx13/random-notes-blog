# Jekyll


## Quick Start

Create a new Jekyll site at ./myblog.
jekyll new myblog
Change into your new directory.
cd myblog
Build the site and make it available on a local server.
bundle exec jekyll serve
Browse to http://localhost:4000

##  O que é Jekyll

**Minhas Observações**

Uma alternativa ao WordPress sem acesso ao banco. Para criaçâo de págians staticas somente.

O mais legal é que cada vez que algum arquivo nesse diretório for modificado, o Jekyll recria o site a partir dele

**O que é**

O Jekyll é um gerador de sites estáticos – de fato, ele é o mais popular dentre eles. Um site estático não possui componentes rodando no lado do servidor: ele usa tecnologias web padrão (HTML5, JS, CSS) e não interage com componentes dinâmicos (um banco de dados, por exemplo).

É versátil, podendo ser usado para criar blogs, landing pages, sites institucionais, entre outros. O conteúdo é criado através de simples arquivos de texto no formato MarkDown. Cada vez que você atualiza estes arquivos, estes são compilados (transformados) em um site completo.

Os sites criados com esta plataforma podem ser hospedados em qualquer provedor de hospedagem, mesmo aqueles sem suporte para linguagens de programação no lado do servidor (PHP, JSP, ASP.NET e outros).

**Contra**

Se você precisa de qualquer tipo de interação que envolva o servidor, manipule banco de dados etc, o Jekyll não pode ser usado para isso. É possível integrar com outras tecnologias, como APIs e serviços de armazenamento na nuvem, mas por si só, o Jekyll não oferece este recurso.

Além disso, se você está desenvolvendo um site para um cliente, e existe uma expectativa de que o cliente mantenha o conteúdo do site, ele teria que usar o terminal e instalar algumas ferramentas de linha de comando…



## Links de Temas

**Gratuitos**

+ http://jekyllthemes.org/
+ https://jekyllthemes.io/
+ http://themes.jekyllrc.org/
+ http://themes.jekyllrc.org/

**Pagos**

+ https://themeforest.net/category/static-site-generators/jekyll

**Links em Português**

+ https://king.host/blog/2018/09/criando-sites-estaticos-com-jekyll/
+ https://jtemporal.com/do-tema-ao-ar/

## Instalação

### Pré-Requisitos

+ Ruby version 2.5.0 or above, including all development headers (ruby version can be checked by running ruby -v)
  + `ruby -v` acima de 2.5
+ RubyGems (which you can check by running gem -v)
  + `gem -v`
+ GCC and Make (in case your system doesn’t have them installed, which you can check by running gcc -v,g++ -v and make -v in your system’s command line interface)
  + `gcc -v`

### Ubuntu

**Links úteis**

+ https://www.edivaldobrito.com.br/como-instalar-o-ruby-version-manager-no-ubuntu/
+ https://linuxize.com/post/how-to-install-ruby-on-ubuntu-18-04/
+ https://zoomadmin.com/HowToInstall/UbuntuPackage/ruby2.5

**Intalar**


Before we install Jekyll, we need to make sure we have all the required dependencies.

```sh
sudo apt-get install ruby-full build-essential zlib1g-dev
```
É necessário uma versão ` > ruby2.4.0`

It is best to avoid installing Ruby Gems as the root user. Therefore, we need to set up a gem installation directory for your user account. The following commands will add environment variables to your ~/.bashrc file to configure the gem installation path. Run them now:

```sh
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Finally, install Jekyll:

```sh
$ gem install jekyll bundler
```

That’s it! You’re ready to start using Jekyll.

### Outros código úteis (caso der problema)

```sh
$ sudo snap install ruby --classic
```


```sh
# Instalado ruby-switch
$ ruby-switch --list
```

```sh
$ rbenv install -l

$ rbenv install 2.6.6
```

```sh
$ sudo apt-get update -y
```

```sh
$ sudo apt-get install -y ruby2.5
```

Instalar `ruby-dev`

```sh
$ sudo apt-get install ruby`ruby -e 'puts RUBY_VERSION[/\d+\.\d+/]'`-dev
```

```sh
$ gem update --system
```

## Criar projeto jekyll

```sh
# criar projeto kekyll na pasta /myblog
$ jekyll new myblog

# entrar 
$ cd myblog/

# Executar
$ bundle exec jekyll serve
```

