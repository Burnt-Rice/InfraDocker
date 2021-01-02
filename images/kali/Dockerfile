FROM kalilinux/kali-rolling:latest


RUN set -x \ 
    && echo '[+]Updating Kali' \
    && DEBIAN_FRONTEND='noninteractive' apt update -qy  \
    && echo '[+] Done'

RUN set -x \ 
    && echo '[+]Installing Tools' \
    && DEBIAN_FRONTEND='noninteractive' apt install kali-tools-top10 -qy \
    openssh-server \
    tmux \
    dirbuster \
    gobuster \
    && echo '[+] Done'


CMD ["/bin/bash"]
