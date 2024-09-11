# React + Vite

(avoir node de deja installé -> node -v)</br>
<b> Si pas node d'installé </b></br>
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt-get install -y nodejs</br>

npm create vite@latest projet1 -- --template=javascript -- --jsx=swc
</br>
<b> Initialisation </b>
</br>
npm create vite@latest projet1 -- --template react-swc

cd projet1

git clone https://github.com/crosskicker/TodoListReact.git

npm install

npm install -D sass

(pour plus tard) :

npm install react-hook-form

npm install @hookform/resolvers yup

npm i react-router-dom

</br>
<b> Lancement  </b>
</br>
npm run dev 

http://localhost:5173



This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

# Docker 🖥️ 🐳

#cheatsheet #essentialguide

[Dockerfile](https://www.notion.so/Dockerfile-3743f45a6988410cafd1cf74df9cc318?pvs=21)

[Docker compose](https://www.notion.so/Docker-compose-8e4d17290dd04f2c8f51c3d867619f58?pvs=21)

### To import an image

```bash
$ docker pull <image_name>
```

### To run a container

```bash
$ docker run [OPTIONS] <image_name> [COMMAND] [ARG...]
```

We can add options:

- -it                 →    run the container in interactive mode with a pseudo-TTY
- --name         →    give a name to the container
- -p                 →    map a container port to a host port (`HOST_PORT:CONTAINER_PORT`)
- -v                 →    mount a host directory as a data volume in the container
- --network    →    specify the network mode for the container

***Some exemples :***

Expose and map a port from the container to the host:

```bash
$ docker run -p 8080:80 <image_name>
```

To persist data or share files between the host and the container

```bash
$ docker run -v /host/data:/container/data <image_name> ls /container/data
```

To start a container with an interactive shell

```bash
$ docker run -it <image_name> /bin/bash
```

Specify a network for the container to connect to

```bash
$ docker run --network <network_name> nginx
```

### To see the running container

```bash
$ docker ps  {options...}
```

We can add options for :

- -a    →    shows us all the containers, stopped or running.
- -l     →    shows us the latest container
- -q    →    shows only the id of the container

### To stop a container

```bash
$ docker stop <container_ID>
```

### To start a container

```bash
$ docker start <container_ID>
```

### To delete a container

```bash
$ docker rm {options} <container_name or ID>
```

We can add options :

- -f    →    remove the container forcefully
- -v   →    remove the volumes
- -l    →    remove the specific link mentionned

### To see our images

```bash
$ docker images
```

### To execute command in a running container

```bash
$ docker exec [OPTIONS] <container_name> <command> [ARG...]
```

We can add options :

- -i    →    keep STDIN open even if not attached
- -t    →    allocate a pseudo-TTY, useful for running commands that require an interactive shell
- -e   →    set environment variables
- -w   →    set the working directory inside the container

***Some exemples :***

To access a bash shell inside a container

```bash
$ docker exec -it <container_name> /bin/bash
```

Run a command without needing an interactive shell

```bash
$ docker exec <container_name> ls /app
```

You can pass environment variables to the command

```bash
$ docker exec -e MY_VAR=value <container_name> printenv MY_VAR
```

Change the working directory for a command

```bash
$ docker exec -w /app CONTAINER_NAME ls
```
