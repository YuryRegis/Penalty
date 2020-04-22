# Penalty - Simulador de Penaltes escrito em C com interface GTK+
Aplicação em desenvolvimento...

## Compilar
As opções -O3 e -s são para otimizações e eliminar símbolos não necessários no arquivo binário final.
```
gcc -O3 -s -o executavel jogo.c  `pkg-config --cflags --libs gtk+-2.0` 
```

## Icone Executavel / Lançador Desktop

Edite o arquivo `Penalty.desktop`, editando as linhas 5 e 6 para o diretório onde encontra o seu arquivo `icon.png` e o `executavel`. Após editado, mova o arquivo `Penalty.desktop` para o diretório de aplicativos da sua distribuição `/usr/share/applications/`.
```
1. [Desktop Entry]
2. Type=Application
3. Name=Penalty
4. StartupNotify=true
5. Exec=diretorio/do/.../executavel
6. Icon=diretorio/do/arquivo/.../assets/icon.png
```

## Fonte
Programação básica em C: https://bitismyth.wordpress.com/2017/04/22/programacao-grafica-em-c-gnome-tool-kit-gtk/

Documentação GTK2+: https://developer.gnome.org/gtk2/2.24/ 

Documentação GTK3+: https://developer.gnome.org/gtk3/stable/
