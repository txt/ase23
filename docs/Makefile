all : $(shell ls *.md)

*.md : ../README.md Makefile
	echo "$@ ... "
	(cat $< | gawk 'BEGIN {FS="\n";RS=""} {print $0 "\n";exit}'|gawk'{print "  " $0} END{print("\n\n;\n\n")}'  \
	 cat $@ | gawk 'BEGIN {FS="\n";RS=""} NR==1 { print("\n\n"); next} {print $0 ""}') > .tmp;
	mv .tmp $@

