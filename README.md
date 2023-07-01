# Server-Muppet
Serrvidor de Minecraft Configurado no docker
Imagem utilizada: buddyspencer/purpur

IMAGE
```
docker pull buddyspencer/purpur
```

preparação do container
```
docker run \
  --name Minecraft-purpur \
  -e MEMORYSIZE='4G' \
  -v /home/Minecraft-server:/data:rw \
  -p 25565:25565 \
  -p 2083:2083 \
  -p 19132:19132/udp \
  -i buddyspencer/purpur:1.20.1
```
--name \para o nome do container
-e => Para a quantidade de de memoria que deseja alocar ao container
-v => /Caminho-do-diretorio-local:/caminho-dentro-do-Container
-p => Porta (Como padrão a porta fica como TCP, para indicar se aporta é UDP apenas dar um /UDP como mostra acima)
-i => Nomedaimagem/purpur:versaoAtual




