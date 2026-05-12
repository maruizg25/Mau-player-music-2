# Mau-player-music-2

Repositorio secundario de música para [Mau-player](https://github.com/maruizg25/Mau-player).

Aquí solo van MP3s y el índice `music/tracks.json` correspondiente.
El player principal (en el otro repo) lee este `tracks.json` vía
`sources.json` y combina las librerías.

## Agregar música

Igual que en el repo principal:

```bash
brew install yt-dlp jq                              # una sola vez
./add-song.sh "https://www.youtube.com/watch?v=ID"  # una canción
./add-song.sh "https://www.youtube.com/playlist?list=PL..." 30   # primeros 30
```

Y al terminar:

```bash
git add music/ && git commit -m "add: tracks" && git push
```

Apenas haga push, el player principal (https://maruizg25.github.io/Mau-player/)
empieza a mostrar también estas canciones.
