FROM paperist/texlive-ja:latest
RUN wget -P "/sty" "https://raw.githubusercontent.com/h-kitagawa/plistings/master/plistings.sty"
RUN tlmgr update --self
RUN tlmgr install algorithms algorithmicx algpseudocodex geometry latexindent
RUN apt update && apt install -y git locales-all libyaml-tiny-perl libfile-homedir-perl
CMD [ "bin/bash" ]
