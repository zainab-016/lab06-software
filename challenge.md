# Challenge: Install It Yourself

## 1. Install and run htop
**Command:**
`sudo apt install -y htop`

**Run command:**
`htop`

**Answer:** htop displays CPU usage, memory usage, and running processes. Press `q` to exit.

## 2. Check the apache2 version
**Command:**
`apt show apache2`

**Answer:** The available Apache2 package version is shown in the Version field. It can be checked without installing the package.

## 3. Count installed packages
**Command:**
`apt list --installed | wc -l`

**Answer:** This command counts the lines in the installed package list. The result may include a header line.

## 4. Run an Alpine container
**Command:**
`sudo docker run --rm alpine echo "Hello from Alpine"`

**Answer:** Docker runs the Alpine Linux container and prints "Hello from Alpine".

## 5. Find Docker's key and sources files
**Commands:**
`ls -l /etc/apt/keyrings/docker.asc`

`cat /etc/apt/sources.list.d/docker.sources`

**Answer:**
- Docker key: `/etc/apt/keyrings/docker.asc`
- Docker sources file: `/etc/apt/sources.list.d/docker.sources`

## 6. Remove htop
**Commands:**
`sudo apt remove -y htop`

`hash -r`

`which htop`

**Answer:** The remove command uninstalls htop. `hash -r` clears Bash's remembered command locations, and `which htop` checks whether the executable is still available.
