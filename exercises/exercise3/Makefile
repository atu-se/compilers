exercise3: calc_infix.lex.c calc_infix.tab.c calc_infix.tab.h
	gcc -o infix calc_infix.tab.c calc_infix.lex.c -ll -lm

example3.c example3.tab.h: calc_infix.y
		bison -d calc_infix.y

calc_infix.lex.c: example3.tab.h example3.l
	flex -o example3.lex.c example3.l


clean:
	rm calc calc.tab.c calc.lex.c calc.tab.h calc_infix.lex.c calc_infix.tab.c calc_infix.tab.h
