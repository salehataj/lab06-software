
# Lab 06 Challenge: Install It Yourself

## 1. Install and Remove htop
Installed htop using `sudo apt install -y htop`.
Ran `htop` to view system processes and pressed `q` to exit.
Removed htop using `sudo apt remove -y htop`.
Ran `hash -r` and verified that htop was no longer available.

## 2. Apache Package Version
Command: `apt show apache2 | grep -m1 '^Version:'`
Version found: `2.4.66-2ubuntu2.6`
The Apache package version was checked without installing Apache.

## 3. Installed Package Count
Command: `apt list --installed | wc -l`
Output: `734`
The command returned 734.

## 4. Docker Alpine Container
Command: `sudo docker run --rm alpine echo "Hello from Alpine"`
Output: `Hello from Alpine`
The Alpine image was downloaded, and the container ran successfully.

## 5. Docker Repository Files
Signing key: `/etc/apt/keyrings/docker.asc`
Repository configuration: `/etc/apt/sources.list.d/docker.sources`
Both files were verified using the `ls -l` command.

## 6. Verify htop Removal
Command: `sudo apt remove -y htop`
Then ran `hash -r` and executed `htop`.
The terminal reported that the htop command was not found, confirming its removal.

