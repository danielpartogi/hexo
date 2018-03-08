---
title: Github Tutorial -dudu-
---

---
> ### Pertama dari yang pertama
---
download dulu gitnya :
1. **[Windows](http://msysgit.github.io/)**
2. **[OSX](http://git-scm.com/download/mac)**
3. **[Linux](http://git-scm.com/book/en/Getting-Started-Installing-Git)**

***
> ### Memulai Git
***

untuk memulai git kita perlu menginisiasi git tersebut di folder kita, dengan command seperti dibawah ini.

    git init

nb : *pastikan sudah berada di folder yang akan dikirim ke github di cmdnya*

*** 
> ### Add&Commit
***

Ketika kita menambahkan file, misalnya syalala.txt maka kita perlu menambahkannya di git, supaya masuk ke lognya maka perlu add&commit. perintahnya adalah `git add(spasi)nama file` dan `commit -m "isinya"` contohnya seperti dibawah ini bila kita menambahkan file syalala.txt:

    add syalala.txt

lalu dilanjutkan dengan

    commit -m "menambahkan file syalala.txt

maka itu artinya kita sudah meng-track file syalala.txt di git kita.

***
> ### Menambahkan File ke Github
***

Untuk menambahkan file tersebut kita hanya perlu menggunakan:

    git push origin master

nb: *ini berlaku jika file yang mau kita kirim ada di branch master*

karena kita akan menambahkan file kita ke server github, misalkan kita akan menambahkan file tersebut ke repository dengan link https://github.com/danielpartogi/hexo.git

maka untuk menambahkannya dengan perintah :

    git remote add origin https://github.com/danielpartogi/hexo.git

baru dilanjutkan dengan perintah seperti diatas yaitu :

    git push origin master



***
> ### Branch
***

berguna untuk menyimpan file yang akan kita edit/perbaharui, dimana nanti file tersebut besifat tersembunyi. metode *branch* sangat berguna bila kita ingin kembali ke versi sebelumnya. Untuk menggunakannya dengan cara :

    git checkout -b nama branchnya

contohnya

    git checkout -b backed

bila ingin pindah branch hanya perlu menggunakan `git checkout <nama filenya>`

***
> ### Pull & Merge
***

pull berguna untuk meng-update file local kita, dimana nanti file yang berada di github akan kita update terlebih dahulu ke directory kita. dengan command `git pull` Dan untuk menyatukan branch yang berbeda dengan branch yang saat ini kita menggunakan `git merge <branch>`

***
> ### LOG
***

log melihat aktivitas yang telah dilakukan seseorang terhadap file yang ada. dapat dilihat dengan perintah

    git log

maka nanti dia akan menampilkan seluruh aktivitas yang ada, serta kode commit dimana nanti kita bisa kembali ke versi log/aktivitas yang telah dibuat seseorang dengan perintah

    git checkout <kodenya>

kodenya minimal hanya butuh 4 angka didepannya.

***
> ### TAG
***

dengan tag kita bisa menandai versi dari file tersebut. contohnya kita ingin menambahkan 1.0.0 maka kita hanya perlu perintah

    git tag 1.0.0 <kodelog>

kode log itu maksudnya adalah kode commit yang ada saat kita menggunakan git log.

