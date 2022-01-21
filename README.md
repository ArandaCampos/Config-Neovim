## Config-Neovim

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=FINALIZADO&color=yellowgreen&style=for-the-badge)   ![Badge versionamento](http://img.shields.io/static/v1?label=VERSAO&message=1.0&color=sucess&style=for-the-badge)

Esse script configura o NeoVim. Aperfeiçoando-o, adicionando novas ferramentas, e adaptando-o para programadores 👨‍💻.

## Pré-requisitos

### Python e a biblioteca pynvim

    $ sudo apt install python3-pip
    $ pip install pynvim
> Instalação do python, pip, e a biblioteca pynvim

### Nodejs

    $ reset
> Fecha o terminal atual e abra um novo.

    $ nvm install --lts
> Instalação do Nodejs

    $ sudo add-apt-repository ppa:neovim-ppa/unstable
    $ sudo apt-get update
    $ sudo apt-get install neovim
> Intalação do neovim

## Instalação

    $ cd ~/.config/
> Entra no diterótio .config

    $ mkdir nvim
 > Cria o diretório nvim

    $ git clone https://github.com/ArandaCampos/Config-Neovim.git nvim
> Clona o script para a pasta nvim

    $ iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni "$(@($env:XDG_DATA_HOME, $env:LOCALAPPDATA)[$null -eq $env:XDG_DATA_HOME])/nvim-data/site/autoload/plug.vim" -Force

> Instala um instalador de Pluggins
 
    $ nvim nvim/init.vim
> Pelo Neovim, abre o arquivo de configuração

Com o arquivo aberto, digite `:PlugInstall` para instalar todos os pluggins do script

![nvim](https://user-images.githubusercontent.com/87876734/147983057-1f35ff5c-da58-4490-9974-d29922b86904.gif)

Feche e salve o nvim `:wq`. 

Ele já estará pronto para codar! 👨‍💻
