default: radii derot

radii:
	g++ -I/usr/include/opencv4/ radii_check.cpp -o radii_check -L`pkg-config --libs opencv4`

derot:
	g++ -I/usr/include/opencv4/ derot.cpp -o derot -L`pkg-config --libs opencv4`

install-bin: radii derot
	mkdir -p /var/www/dpr-dev.epss.ucla.edu/bin
	cp radii_check /var/www/dpr-dev.epss.ucla.edu/bin/radii_check
	cp derot /var/www/dpr-dev.epss.ucla.edu/bin/derot
