##### Level 0
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
bandit0
cat readme
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
```

##### Level 1
```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
ls && cat ./-
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
```

##### Level 2
```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
cat ./spaces\ in\ this\ filename
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
```

##### Level 3
```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
cat inhere/.hidden
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
```

##### Level 4
```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
cat inhere/-file07
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
```

##### Level 5
```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
find ./inhere/ -size 1033c -readable \! -executable
cat ./inhere/maybehere07/.file2
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
```

##### Level 6
```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
cd /
find -user bandit7 -group bandit6 -size 33c
cat ./var/lib/dpkg/info/bandit7.password
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
```

##### Level 7
```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
grep "millionth" data.txt
TESKZC0XvTetK0S9xNwm25STk5iWrBvP
```

##### Level 8
```bash
ssh bandit8@bandit.labs.overthewire.org -p 2220
# Find a unique line of text
sort data.txt | uniq -u
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
```
```python
with open('data.txt', 'r') as file:
    file = sorted(file.readlines())
    
counter, previous = 0, None

for line in file:
    line = line.strip()
    if previous is None:
        previous = line
    if previous == line:
        counter += 1
    else:
        print(counter, previous)
        counter, previous = 1, line
```

##### Level 9
```bash
ssh bandit9@bandit.labs.overthewire.org -p 2220
# Hexdump a binary file
xxd data.txt
strings data.txt | grep =*
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
```

##### Level 10
```bash
ssh bandit10@bandit.labs.overthewire.org -p 2220
# Decode Base64
base64 -d data.txt
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
```

##### Level 11
```bash
ssh bandit11@bandit.labs.overthewire.org -p 2220
# Decode Rot13
cat data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
```

##### Level 12
```bash
ssh bandit12@bandit.labs.overthewire.org -p 2220
# Do the right extraction
sudo apt install dtrx
dtrx --one rename data.gz
dtrx --one rename data
dtrx --one rename data.1
dtrx --one rename data.2
dtrx --one rename data.3
dtrx --one rename data.4
cat data.4.1
wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
```

##### Level 13
```bash
ssh bandit13@bandit.labs.overthewire.org -p 2220
ssh -i sshkey.private bandit14@localhost -p 2220
```

##### Level 14
```bash

```