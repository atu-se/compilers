all:	a.out

a.out:	lex.yy.c
	gcc lex.yy.c -lfl

lex.yy.c: 	exercise3.l
	flex exercise3.l
