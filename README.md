# Penalty - Siimulador de Penaltes escrito em C com interface GTK+

## Compilar
```gcc -O3 -s -o executavel jogo.c  \`pkg-config --cflags --libs gtk+-2.0\` ```

## Icone Executavel / Lançador Desktop

Edite o arquivo `Penalty.desktop`, editando as linhas 5 e 6 para o diretório onde encontra o seu arquivo `icon.pmg` e o `executavel`. Após editado, mova o arquivo `Penalty.desktop` para o diretório de aplicativos da sua distribuição `/usr/share/applications/`.
```
1. [Desktop Entry]
2. Type=Application
3. Name=Penalty
4. StartupNotify=true
5. Exec=diretorio/do/.../executavel
6. Icon=diretorio/do/arquivo/.../assets/icon.png
```