### Tugas keenam
* Buatlah sebuah file dengan nama `nama-kalian.md`, kemudian isilah
file tersebut dengan format seperti berikut :
```
Nama : Nama Lengkap
Kelas/Tingkat :
Moto :
```
* Untuk mengerjakan latihan tersebut lakukan langkah-langkah berikut ini :
  - Install Git
  - Konfigurasi Awal
    ```
    $ git config --global user.name "Nama Lengkap"
    $ git config --global user.email "user@example.com"
    $ cat ~/.gitconfig
    ```
  - Generating `public_key`
    ```
    $ ssh-keygen -t rsa -C "email@example.com"
    $ cp ~/.ssh/id_rsa.pub ~/.ssh/nama-kalian.pub
    $ scp ~/.ssh/nama-kalian.pub student@git.gitserver:/tmp/
    ```
  - Create Repository
    ```
    $ git clone git@git.gitserver:/mahasiswa/nama-kalian.git
    $ cd nama-kalian/
    $ touch nama-kalian.md
    $ notepad.exe nama-kalian.md
    ```
    Simpan, kemudian lakukan commit :
    ```
    $ git add nama-kalian.md
    $ git commit -m "mengumpulkan tugas"
    $ git push origin master

    ```
