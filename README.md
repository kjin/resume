# Kelvin Jin's Resume

## Setup

### Ubuntu

First, get TexLive from their website (don't use the Ubuntu dist version)

	wget http://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz
	tar -zxvf install-tl-unx.tar.gz

Might want to create `/usr/local/texlive` beforehand and temporarily set up 777 permissions to allow setup to proceed without permission problems (is this the best/only way to do it? not sure)

In install-tl, Use `S` and select the small package (`c`). Then go ahead and install it (make sure to add binaries to `PATH` once complete)

Download and install the TTF Fontin font @ http://www.exljbris.com/fontin.html (the font creator does not want direct links to TTF files)

	unzip fontin-pc.zip
	sudo mv Fontin-* /usr/share/fonts/truetype

Finally, we've got to install some packages:

	tlmgr install preprint
	tlmgr install titlesec

## Compiling the PDF file

	xelatex resume.tex

