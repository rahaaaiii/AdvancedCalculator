fb1-5: fb1-5.l fb1-5.y
	bison -d fb1-5.y
	flex fb1-5.l
	gcc -o $@ fb1-5.tab.c lex.yy.c -lfl
clean:
	for file in fb1-5.tab.c fb1-5.tab.c lex.yy.c fb1-5; do \
		if [ -e $$file ]; then rm $$file; fi; \
	done

.SILENT: clean