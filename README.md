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
* **Password Saat Ini:** `bandit1`

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
* **Password Saat Ini:** `bandit2`

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
* **Password Saat Ini:** `bandit3`

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

