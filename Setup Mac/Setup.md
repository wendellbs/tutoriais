
# Setup Mac

##  Setup terminal
- [ ] [iTerm](https://www.iterm2.com/downloads.html)
- [ ] [Homebrew]([https://brew.sh/index_pt-br](https://brew.sh/index_pt-br))

### Softwares no terminal
- [ ] Git, ZSH, ZSH-Completions, Oh-My-ZSH
```
brew install git
brew install zsh zsh-completions
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
- [ ] Fontes Powerline
```
git clone https://github.com/powerline/fonts.git --depth=1
cd fonts
./install.sh
cd ..
rm -rf fonts
```
- [ ] Ajustas arquivo `~/.zshrc`
```
ZSH_THEME="agnoster"
```
- [ ] Mudar esquema de cores do iterm
	- [Baixar os temas]([schemes.zip](https://github.com/wendellbs/tutoriais/files/3055780/schemes.zip))
	- Importar o tema `Brogrammer.itermcolors` no iTerm
	- Mudar cor do auto-suggestion:
![Screen Shot 2019-04-08 at 15 39 08](https://user-images.githubusercontent.com/13970064/55748231-7af17100-5a14-11e9-9cf3-39af7bca0976.png)
	- Mudar schema de keys:
![Screen Shot 2019-04-08 at 15 50 45](https://user-images.githubusercontent.com/13970064/55748865-1d5e2400-5a16-11e9-8b58-232b078a5f5f.png)

- [ ] Esconder nome do PC no terminal
	- Abrir ~/.zshrc
	- Inserir:
	``` export DEFAULT_USER="$(whoami)" ```
- [ ] Scheme Color no VI
	- Abrir/ Criar o arquivo ~/.vimrc e inserir:
```
filetype plugin indent on
syntax on
```

## VSCode
- [Download]([https://code.visualstudio.com/Download](https://code.visualstudio.com/Download))
- Baixar a extensão `Settings Sync` e sincronizar as configurações do VSCode:![image](https://user-images.githubusercontent.com/13970064/55752477-847fd680-5a1e-11e9-9203-8fb61a6ca5c1.png)


## Outros softwares
- [ ] [Docker]([https://hub.docker.com/editions/community/docker-ce-desktop-mac](https://hub.docker.com/editions/community/docker-ce-desktop-mac))
- [ ] [Node]([https://nodejs.org/en/download/](https://nodejs.org/en/download/))

## Ambiente Python
- [ ] Instalar Python3: `brew install python3`
- [ ] Instalar virtualenv: `pip3 install virtualenv`
- [ ] Criar alias do `pip3` para `pip`:
	- Adicionar a seguinte linha no arquivo ~/.zshrc: ``

## Referências
[Jazz Up Your “ZSH” Terminal In Seven Steps — A Visual Guide](https://medium.freecodecamp.org/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38)
