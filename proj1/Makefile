#/*
# *********************************************
# *  314 Principles of Programming Languages  *
# *  Fall 2017                                *
# *  Authors: Ulrich Kremer                   *
# *********************************************
# */

CCFLAGS = -ggdb -Wall

all: compile constfolding strengthreduct

compile: Compiler.c InstrUtils.c InstrUtils.h Utils.c Utils.h
	gcc $(CCFLAGS) Compiler.c InstrUtils.c Utils.c -o compile

constfolding: ConstFolding.c InstrUtils.c InstrUtils.h Utils.c Utils.c
	gcc $(CCFLAGS) ConstFolding.c InstrUtils.c Utils.c Utils.h -o constfolding

strengthreduct: ConstFolding.c InstrUtils.c InstrUtils.h Utils.c Utils.c
	gcc $(CCFLAGS) StrengthReduction.c InstrUtils.c Utils.c Utils.h -o strengthreduct -lm

clean:
	rm -rf compile constfolding strengthreduct tinyL.out

