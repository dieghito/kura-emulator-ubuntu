## Kura emulator on Ubuntu
Questa immagine è stata creata per poter utilizzare l'emulatore di Eclipse Kura su un sistema operativo basato su Debian/Ubuntu.

## Build image
Per poter buildare l'immagine è sufficiente lanciare questo comando:

```
docker build --rm -f DockerFile -t dieghito85/kura-emulator-ubuntu:latest .
```

## Run rapido
L'immagine non ha bisogno di particolari lavorazioni, non ha a disposizione la web console, ma è possibile usare la console interna. Quindi per effettuare il Run del container è sufficiente lanciare il seguente comando:

```
docker run -d --name=kura-emulator -p 8080:8080 -p 1450:1450 dieghito85/kura-emulator-ubuntu
