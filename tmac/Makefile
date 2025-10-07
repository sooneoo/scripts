TEX_MACRO_PATH=$$(kpsewhich -var-value=TEXMFHOME)/tex/plane/tmac


all: env install update_tex


install:
	cp -v ./tmac.tex $(TEX_MACRO_PATH)/
	cp -rv ./amsfonts/fonts ~/texmf/
	cp -rv ./amsfonts/tex ~/texmf


update_tex:
	texhash ~/texmf
	mktexlsr ~/texmf


env:
	mkdir -pv ~/texmf
	mkdir $(TEX_MACRO_PATH) -vp

