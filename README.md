# Netcat tool for Network pentesting

usage: `netcat.py [-h] [-c] [-e EXECUTE] [-l] [-p PORT] [-t TARGET] [-u UPLOAD]`

Blackarcher Net Tool

**options:**
 ` -h, --help` show this help message and exit
 `-c, --command ` command shell
 `-e EXECUTE, --execute EXECUTE`
 execute specified command
 `-l, --listen` listen
 `-p PORT, --port PORT` specified port
`-t TARGET, --target TARGET`
 specified IP
 `-u UPLOAD, --upload UPLOAD`
 upload file

**Example:**

`netcat.py -t 192.168.0.1 -p 5555 -l -c # command shell
netcat.py -t 192.168.0.1 -p 5555 -l -u=file.txt # upload file
netcat.py -t 192.168.0.1 -p 5555 -l -e "cat /etc/passwd" # execute command
echo 'ABC' | ./netcat.py 192.168.0.1 -p 135 # echo text to server port 135
netcat.py -t 192.168.0.1 -p 5555 # connect to server`
