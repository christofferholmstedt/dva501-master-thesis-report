LaTeX text for my master thesis report
===============================================================

### About this report
This git repository includes my report(s) from my master thesis work
done during the spring of 2014 concerning "Virtual Network Protocol".

### How to generate PDF in Ubuntu 12.04
```
cd /directory/with/.tex_file
pdflatex sigproc-sp.tex
bibtex sigproc-sp.aux
pdflatex sigproc-sp.tex
pdflatex sigproc-sp.tex
```
All latex commands are run with the make file located next to the main files.
```
make
```
A third option is to use Vagrant together with Virtualbox if you don't
want to install all the Latex dependencies on your development machine.
The Vagrantfile is configured to install a basic Ubuntu 12.04 LTS server
machine and the necessary packages to generate all reports. Just the
following command and wait.
```
vagrant up
```

