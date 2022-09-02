# Post Bootcamp Review

Supaya temen-temen memahami apa yang telah pemateri sampaikan, silahkan kerjakan task berikut

## Task 1 (Virtualization)

- Buatlah sebuah VM di Nutanix Cluster yang telah di berikan dengan kententuan
  - username: `<github_user>` contoh `dimasm93`
  - hostname: `<email_without_at>` contoh `dimas.tabeldata.com`
  - OS: `ubuntu-20.04` atau `centos-7`
- Install webserver `nginx`
  - Deploy aplikasi dalam folder `webapp` ke webserver nginx

## Task 2 (Container)

Berdasarkan task no 1, buatlah versi containernya: 

1. build docker image dengan nama `<username>/post-bootcamp`
2. tag docker image yang telah dibuat dengan nama baru `10.42.29.110:5000/<username>/post-bootcamp`
3. Jalankan containernya berdasarkan docker image tersebut.
4. Setelah ok, semuanya jalan. coba push ke docker registry di nutanix cluster
5. Kemudian check di registry dengan akses browser `10.42.29.110:5000/v2/_catalog`
6. Buat docker-compose filenya, kemudian simpan dalam folder `tasks` dengan nama `docker-compose.yaml`

## Task 3 (Orchestration Container System)

1. Buatlah kubernetes workload resources deployment untuk container tersebut
2. Expose deployment tersebut menggunakan service dengan type NodePort

## Task 4 (CI/CD)

1. Berdasarkan task 2, 3 coba buatlah automationnya menggunakan `gitlab-ci.yml`
2. Untuk build, push ke docker registry
3. Untuk deploy ke kubernetes cluster
