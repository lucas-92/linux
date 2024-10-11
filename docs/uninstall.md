## Desinstalar via sudo apt remove:
```
sudo apt remove nome-do-pacote-instalado
```

### Para remover também os arquivos de configuração:
```
sudo apt purge nome-do-pacote-instalado
```

## Desinstalar via flatpak uninstall:
```
flatpak uninstall nome-do-pacote-instalado
```

## Remover os arquivos de configuração via rm -rf
```
rm -rf ~/.config/nome-do-pacote-instalado/
rm -rf ~/.cache/nome-do-pacote-instalado/
```

## Remover pacotes com sudo apt autoremove
Remover os pacotes que não são mais necessários:
```
sudo apt autoremove
```
