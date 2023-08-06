Level 0
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
bandit0
cat readme
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
```

Level 1
```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
ls && cat ./-
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
```

Level 2
```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
cat ./spaces\ in\ this\ filename
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
```

Level 3
```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
cat inhere/.hidden
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
```

Level 4
```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
cat inhere/-file07
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
```

Level 5
```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
find ./inhere/ -size 1033c -readable \! -executable
cat ./inhere/maybehere07/.file2
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
```

Level 6
```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
cd /
find -user bandit7 -group bandit6 -size 33c
cat ./var/lib/dpkg/info/bandit7.password
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
```

Level 7
```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
grep "millionth" data.txt
TESKZC0XvTetK0S9xNwm25STk5iWrBvP
```

Level 8
```bash
ssh bandit8@bandit.labs.overthewire.org -p 2220
sort data.txt | uniq -u
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
```
```python
# find a unique line of text
data = []
with open('data.txt', 'r') as file:
    file = file.readlines()
    for line in file:
        data.append(line.strip())

data = sorted(data)
counter = 0
previous = None

for line in data:
    if previous is None:
        previous = line
    elif previous == line:
        counter += 1
    else:
        print(previous, counter)
        counter = 1
        previous = line
```

Level 9
```

```