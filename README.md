 CODE=$(curl -sc /tmp/cookie "https://drive.google.com/uc?export=download&id=1-TB_9RDhkwfh0XrZipyCBSJE05FvTaOG" | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')

 curl -JO -Lb /tmp/cookie  "https://drive.google.com/uc?export=download&confirm=t&id=1-TB_9RDhkwfh0XrZipyCBSJE05FvTaOG"
