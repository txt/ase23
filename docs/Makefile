all : $(shell ls *.md)

ONE=cat $< | gawk 'BEGIN {FS="\n";RS=""} {print $$0 "\n"; exit}' | gawk '{print "  " $$0} END{print("\n\n")}' 
TWOPLUS=cat $@ | gawk 'BEGIN {FS="\n";RS=""} NR==1 { print("\n\n"); next} {print $$0 ""}'

*.md : ../README.md Makefile
	echo "$@ ... "
	($(ONES);  $(TWOPLUS)) > .tmp
	mv .tmp $@

