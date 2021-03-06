# Makefile to download themes for emacs

# Copyright (C) 2014 Johannes Rainer

# Author: Johannes Rainer

## Set most variables in Makeconf
include ../Makeconf

#PREFIX=~/.emacs.d
#EMACS=emacs
#ELCC=$(EMACS) -batch -q -no-site-file -no-init-file
#RSYNC=rsync -n -avu --exclude="*~"

# where to put the themes.
DESTDIR=${PREFIX}/themes
AZ=tmp/anti-zenburn-theme
LEUVEN=tmp/emacs-leuven-theme
NOCTILUX=tmp/noctilux-theme
SOFTMORNING=tmp/soft-morning-theme
SOLARIZED=tmp/solarized-emacs
ZENBURN=tmp/zenburn-emacs
PROF=tmp/emacs-professional-theme
MOE=tmp/moe-theme.el
# FLATUI=tmp/emacs-flatui-theme
FLATJO=tmp/flatui-emacs
KAOLIN=tmp/emacs-kaolin-themes
MATERIAL=tmp/emacs-material-theme
MONOKAI=tmp/monokai-emacs
SANITYINC=tmp/color-theme-sanityinc-tomorrow
TANGOTANGO=tmp/color-theme-tangotango
TANGOPLUS=tmp/tango-plus-theme
GITHUB=tmp/color-theme-github
ATOMONE=tmp/atom-one-dark-theme
DRACULA=tmp/dracula-theme
GRUVBOX=tmp/gruvbox-emacs
GRUVBOX2=tmp/emacs-theme-gruvbox
AMPLE=tmp/ample-theme
CREAMSODY=tmp/emacs-theme-creamsody
ONE=tmp/emacs-one-themes
SPACEMACS=tmp/spacemacs-theme
##HIGHCONTRAST=tmp/replace-colorthemes

all : anti-zenburn emacs-leuven-theme noctilux-theme soft-morning-theme solarized-emacs zenburn-emacs emacs-professional moe-theme flatui-emacs monokai tangotango tangoplus github atom-one-dark-theme gruvbox ample creamsody material kaolin one sanityinc spacemacs gruvbox2 melpa

goodones : anti-zenburn noctilux-theme solarized-emacs zenburn-emacs flatui-emacs monokai gruvbox kaolin one spacemacs gruvbox2

.PHONY : anti-zenburn clean emacs-leuven-theme noctilux-theme soft-morning-theme solarized-emacs zenburn-emacs flatui-emacs monokai tangotango tangoplus github gruvbox2

ample :
	@echo ----- installing ample-theme...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${AMPLE} ]; then cd tmp && git clone https://github.com/jordonbiondo/ample-theme; fi
	cd ${AMPLE} && git pull
	cp -p ${AMPLE}/*.el ${DESTDIR}
	@echo ----- Done.

anti-zenburn :
	@echo ----- installing anti-zenburn-theme...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${AZ} ]; then cd tmp && git clone https://github.com/m00natic/anti-zenburn-theme.git; fi
	cd ${AZ} && git pull
#	${EMACS} -Q -L ${AZ} -batch -f batch-byte-compile ${AZ}/*.el
#	mv ${AZ}/*.elc ${DESTDIR}
	cp -p ${AZ}/*.el ${DESTDIR}
	@echo ----- Done.

atom-one-dark-theme :
	@echo ----- installing atom-one-dark-theme...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${ATOMONE} ]; then cd tmp && git clone https://github.com/jonathanchu/atom-one-dark-theme; fi
	cd ${ATOMONE} && git pull
	cp -p ${ATOMONE}/*.el ${DESTDIR}
	@echo ----- Done.

dracula-theme :
	@echo ----- installing dracula-theme...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${DRACULA} ]; then cd tmp && git clone https://github.com/dracula/dracula-theme/; fi
	cd ${DRACULA} && git pull
	cp -p ${DRACULA}/*.el ${DESTDIR}
	@echo ----- Done.

creamsody :
	@echo ----- installing creamsody...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${CREAMSODY} ]; then cd tmp && git clone https://github.com/jorainer/emacs-theme-creamsody.git; fi
	cd ${CREAMSODY} && git pull
	cp -p ${CREAMSODY}/*.el ${DESTDIR}
	@echo ----- Done.

emacs-leuven-theme :
	@echo ----- installing emacs-leuven-theme...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${LEUVEN} ]; then cd tmp && git clone https://github.com/jorainer/emacs-leuven-theme; fi
	cd ${LEUVEN} && git pull
#	${EMACS} -Q -L ${LEUVEN} -batch -f batch-byte-compile ${LEUVEN}/*.el
#	mv ${LEUVEN}/*.elc ${DESTDIR}
	cp -p ${LEUVEN}/*.el ${DESTDIR}
	@echo ----- Done.

emacs-professional :
	@echo ----- installing emacs-professional...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${PROF} ]; then cd tmp && git clone https://github.com/juanjux/emacs-professional-theme.git; fi
	cd ${PROF} && git pull
	cp -p ${PROF}/*.el ${DESTDIR}
	@echo ----- Done.

# flatui :
# 	@echo ----- installing flatui-emacs...
# 	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
# 	if [ ! -d tmp]; then mkdir tmp; fi
# 	if [ ! -d ${FLATUI} ]; then cd tmp && git clone https://github.com/MetroWind/emacs-flatui-theme.git; fi
# 	cd ${FLATUI} && git pull
# 	cp -p ${FLATUI}/*.el ${DESTDIR}
# 	@echo ----- Done.

flatui-emacs :
	@echo ----- installing flatui-emacs...
#	dash it, I need dash!
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${FLATJO} ]; then cd tmp && git clone https://github.com/jorainer/flatui-emacs.git; fi
	cd ${FLATJO} && git pull
	cp -p ${FLATJO}/*.el ${DESTDIR}
#	${EMACS} -Q -L ${FLATJO} -batch -f batch-byte-compile ${FLATJO}/*.el
#	mv ${FLATJO}/*.elc ${DESTDIR}
	@echo ----- Done.

github :
	@echo ----- installing github-emacs...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp]; then mkdir tmp; fi
	if [ ! -d ${GITHUB} ]; then cd tmp && git clone https://github.com/dudleyf/color-theme-github.git; fi
	cd ${GITHUB} && git pull
	cp -p ${GITHUB}/*.el ${DESTDIR}
	@echo ----- Done.

gruvbox :
	@echo ----- installing gruvbox...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp]; then mkdir tmp; fi
	if [ ! -d ${GRUVBOX} ]; then cd tmp && git clone https://github.com/jorainer/gruvbox-emacs; fi
	cd ${GRUVBOX} && git pull
	cp -p ${GRUVBOX}/*.el ${DESTDIR}
	@echo ----- Done.

gruvbox2 :
	@echo ----- installing gruvbox...
	if [ ! -d ${DESTDIR}/gruvbox2 ]; then mkdir ${DESTDIR}/gruvbox2; fi
	if [ ! -d tmp]; then mkdir tmp; fi
	if [ ! -d ${GRUVBOX2} ]; then cd tmp && git clone https://github.com/Greduan/emacs-theme-gruvbox; fi
	cd ${GRUVBOX2} && git pull
	cp -p ${GRUVBOX2}/*.el ${DESTDIR}/gruvbox2
	@echo ----- Done.

kaolin :
	@echo ----- installing kaolin...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp]; then mkdir tmp; fi
	if [ ! -d ${KAOLIN} ]; then cd tmp && git clone https://github.com/ogdenwebb/emacs-kaolin-themes.git; fi
	cd ${KAOLIN} && git pull
	cp -p ${KAOLIN}/*.el ${DESTDIR}
	cp -p ${KAOLIN}/themes/*.el ${DESTDIR}
	@echo ----- Done.

material :
	@echo ----- installing material...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${MATERIAL} ]; then cd tmp && git clone https://github.com/cpaulik/emacs-material-theme.git; fi
	cd ${MATERIAL} && git pull
	cp -p ${MATERIAL}/*.el ${DESTDIR}
	@echo ----- Done.

melpa :
	@echo "\n\nPlease install the following theme(s) manually using melpa (M-x list-packages):"
	@echo " - doom-themes"

moe-theme :
	@echo ----- installing moe-theme...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${MOE} ]; then cd tmp && git clone https://github.com/kuanyui/moe-theme.el.git; fi
	cd ${MOE} && git pull
	cp -p ${MOE}/*.el ${DESTDIR}
	@echo ----- Done.

monokai :
	@echo ----- installing monokai...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${MONOKAI} ]; then cd tmp && git clone https://github.com/oneKelvinSmith/monokai-emacs.git; fi
	cd ${MONOKAI} && git pull
	cp -p ${MONOKAI}/*.el ${DESTDIR}
	@echo ----- Done.

noctilux-theme :
	@echo ----- installing noctilux-theme...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${NOCTILUX} ]; then cd tmp && git clone https://github.com/stafu/noctilux-theme.git; fi
	cd ${NOCTILUX} && git pull
#	${EMACS} -Q -L ${NOCTILUX} -batch -f batch-byte-compile ${NOCTILUX}/*.el
#	mv ${NOCTILUX}/*.elc ${DESTDIR}
	cp -p ${NOCTILUX}/*.el ${DESTDIR}
	@echo ----- Done.

one :
	@echo ----- installing one...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${ONE} ]; then cd tmp && git clone https://github.com/balajisivaraman/emacs-one-themes; fi
	cd ${ONE} && git pull
	cp -p ${ONE}/*.el ${DESTDIR}
	@echo ----- Done.


soft-morning-theme :
	@echo ----- installing soft-morning-theme...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${SOFTMORNING} ]; then cd tmp && git clone https://github.com/mswift42/soft-morning-theme.git; fi
	cd ${SOFTMORNING} && git pull
#	${EMACS} -Q -L ${SOFTMORNING} -batch -f batch-byte-compile ${SOFTMORNING}/*.el
#	mv ${SOFTMORNING}/*.elc ${DESTDIR}
	cp -p ${SOFTMORNING}/*.el ${DESTDIR}
	@echo ----- Done.

solarized-emacs :
	@echo ----- installing solarized-emacs...
#	dash it, I need dash!
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${SOLARIZED} ]; then cd tmp && git clone https://github.com/jorainer/solarized-emacs.git; fi
	cd ${SOLARIZED} && git pull
	cp -p ${SOLARIZED}/*.el ${DESTDIR}
#	${EMACS} -Q -L ${SOLARIZED} -batch -f batch-byte-compile ${SOLARIZED}/*.el
#	mv ${SOLARIZED}/*.elc ${DESTDIR}
	@echo ----- Done.

sanityinc :
	@echo ----- installing sanityinc...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${SANITYINC} ]; then cd tmp && git clone https://github.com/purcell/color-theme-sanityinc-tomorrow; fi
	cd ${SANITYINC} && git pull
	cp -p ${SANITYINC}/*.el ${DESTDIR}
	@echo ----- Done.

spacemacs :
	@echo ----- installing spacemacs
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${SPACEMACS} ]; then cd tmp && git clone https://github.com/nashamri/spacemacs-theme; fi
	cd ${SPACEMACS} && git pull
	cp -p ${SPACEMACS}/*.el ${DESTDIR}
	@echo ----- Done.

tangoplus :
	@echo ----- installing tangoplus...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${TANGOPLUS} ]; then cd tmp && git clone https://github.com/tmalsburg/tango-plus-theme.git; fi
	cd ${TANGOPLUS} && git pull
	cp -p ${TANGOPLUS}/*.el ${DESTDIR}
	@echo ----- Done.

tangotango :
	@echo ----- installing tangotango...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${TANGOTANGO} ]; then cd tmp && git clone https://github.com/juba/color-theme-tangotango.git; fi
	cd ${TANGOTANGO} && git pull
	cp -p ${TANGOTANGO}/*.el ${DESTDIR}
	@echo ----- Done.

zenburn-emacs :
	@echo ----- installing zenburn-emacs...
	if [ ! -d ${DESTDIR} ]; then mkdir ${DESTDIR}; fi
	if [ ! -d tmp ]; then mkdir tmp; fi
	if [ ! -d ${ZENBURN} ]; then cd tmp && git clone https://github.com/bbatsov/zenburn-emacs.git; fi
	cd ${ZENBURN} && git pull
	cp -p ${ZENBURN}/*.el ${DESTDIR}
#	${EMACS} -Q -L ${ZENBURN} -batch -f batch-byte-compile ${ZENBURN}/*.el
#	mv ${ZENBURN}/*.elc ${DESTDIR}
	@echo ----- Done.



clean :
	@echo ----- Removing all installed themes...
#	Note, we're removing all *.elc files from DESTDIR!
	rm -Rf ${DESTDIR}/*
	rm -Rf tmp/*
	@echo ----- Done.

