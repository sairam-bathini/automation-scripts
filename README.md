#!/bin/bash
################################
# Author: Sairam
# Version: v1
#
#
#
# This script will help to display odd numbers from 1 to 99
################################


for ((i=1; i<=99; i+=2)) #double The double parentheses (( ... )) are used for arithmetic operations and evaluations in Bash
do
    echo $i
done
