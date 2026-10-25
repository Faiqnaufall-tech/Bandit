# Bandit

### Level 0 - 1
* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`
* **Username:** `bandit0`
* **Password Saat Ini:** `bandit0`

---

### Tujuan 
> membongkar file readme yang didalam nya terdapat password acak

### Perintah & Ekplorasi
**Command yang digunakan:**
```bash
ls
cat

```
---

### Level 1 - 2
* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`
* **Username:** `bandit1`
* **Password Saat Ini:** `6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR`

---

### Tujuan 
> membongkar file dashed (-) yang ada di directory home untuk menemukan password acak

### Perintah & Eksplorasi 
**Command yang digunakan:**
```bash
ls
cat ./-

```
---

### Level 2 - 3
* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`
* **Username:** `bandit2`
* **Password Saat Ini:** `PK8fYLZg2hnHSz83plBL1iEPKdD3QToB`

---

### Tujuan
> membongkar file yang nama file nya di spasi seperti --spaces in this filename--

### Perintah & Eksplorasi
**Command yang digunakan:**
```bash
ls
cat ./--spaces\ in\ this\ filename--

```
---

### Level 3 - 4
* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`
* **Username:** `bandit3`
* **Password Saat Ini:** `7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME`

---

### Tujuan
> membongkar file hidden yang berlapis

### Perintah & Eksplorasi
**Command yang digunakan:**
```bash
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ ls -a
.  ..  ...Hiding-From-You
bandit3@bandit:~/inhere$ du ./...Hiding-From-You
4       ./...Hiding-From-You
bandit3@bandit:~/inhere$ cat ./...Hiding-From-You

```
---

### Level 4 - 5 
* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`
* **Username:** `bandit4`
* **Password Saat Ini:** `xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq`

---

### Tujuan
> membongkar file yang berada di folder inhere yang mana di dalam folder tersebut terdapat banyak file dan harus mencari tahu file mana yang terdapat kode password

### Perintah & Eksplorasi
**Command yang digunakan:**
```bash
bandit4@bandit:~/inhere$ ls -a
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09  .  ..
bandit4@bandit:~/inhere$ file ./*
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
bandit4@bandit:~/inhere$ cat ./-file07

```
---

### Level 5 - 6
* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`
* **Username:** `bandit5`
* **Password Saat Ini:** `6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG`
  
---

### Tujuan
> mencari password di sebuah file yang berada di folder inhere yang mana di folder tersebut terdapat banyak folder. terdapat clue yaitu human-readable, 1033 bytes in size, not executable.

### Perintah & Eksplorasi
**Command yang digunakan:**
```bash
bandit5@bandit:~/inhere$ find . -type f -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
pXa26xhMWaC2SvDotA4r9EgZkulOeSBW
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        bandit5@bandit:~/inhere$
bandit5@bandit:~/inhere$

```
---

