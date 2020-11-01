Start a stopped container

<details><summary>show</summary>
<p>

List stopped containers

```bash
docker ps -a
```

Run a stopped container

```bash
docker start 4ef717e9d2b3
```

Replace 4ef717e9d2b3 with the container ID that has STATUS Exited

List running containers

```bash
docker ps 
```

Take a screen shot of the output and store in Day01/ directory
</p>
</details>

Run a container from ahmedgabercod/clock image in detached mode and attach to it

<details><summary>show</summary>
<p>

```bash
docker run -d ahmedgabercod/clock
```

```bash
docker ps 
```

```bash
docker attach 83eddd360892
```

Replace 83eddd360892 with the container ID on your screen

You should see the out of the clock image
</p>
</details>