# Calc Time

## Introduction

This is a time calculating bash script. It expects an input file of which each line has the 
 form:
 
    {unix timestamp},{START or END},{Some descriptive text for yourself}
 
 I currenlty populate such a file with a command like this:
 
    $> echo "`date +%s`,START,what i am working on" >> this_weeks_file.csv

 Now to parse that CSV with this script run:
 
    $> cat this_weeks_file.csv | ./calc_time

 Produces output like:

    Mon Mar  9 10:34:41 2015 Total: 8.35278
    Tue Mar 10 10:00:00 2015 Total: 7.76222
    Wed Mar 11 10:20:00 2015 Total: 7.02722
    Thu Mar 12 09:40:00 2015 Total: 8.20694
    Fri Mar 13 09:34:44 2015 Total: 1.73667
                             Running Total: 33.0858


## Requirements / Tools Used Internally

- Bash Shell
- Perl
- Awk



