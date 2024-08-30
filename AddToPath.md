# Invoke `pgdiff` Anywhere

## 1. Create and open a script directory.

```bash
mkdir ~/bash/ && cd ~/bash/
```

## 2. Clone the `pgdiff` repo into the directory

```bash
git clone https://github.com/denvaar/pgdiff.git
```

## 3. Copy the working directory

```bash
cd pgdiff && pwd
```

It will look something like this on a Mac:

```bash
/Users/USER/bash/pgdiff
```

## 4. Add directory to path


```bash
export PATH=$PATH:/paste/working/directory/bash/pgdiff
```

## 5. Confirm it works

`cd` to another directory and invoke `pgdiff`

```bash
cd ~/ && pgdiff
```

## 6. ???

## 7. Profit
