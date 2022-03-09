all : ../LICENSE.md $(shell ls *.md)

ONE=cat $< | gawk 'BEGIN {FS="\n";RS=""} {print $$0 "\n"; exit}' | gawk '{print "  " $$0} END{print("")}' 
TWOPLUS=cat $@ | gawk 'BEGIN {FS="\n";RS=""} NR==1 { print(""); next} {print $$0 ""}'

publish:
	$(MAKE) all
	git add *;git commit -am save;git push;git status

../LICENSE.md : ../README.md Makefile; @echo "$@ ... " ; ($(ONE);  $(TWOPLUS)) > .tmp; mv .tmp $@
*.md          : ../README.md Makefile; @echo "$@ ... " ; ($(ONE);  $(TWOPLUS)) > .tmp; mv .tmp $@


