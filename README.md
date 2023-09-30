#!/bin/bash

###########
#Author: Sairam Bathini
#Date: 30-09-2023
#Version: v1
#This script is used to print YES or NO based on the input such as if input is y/Y then output YES, viceversa
###########

read -p 1 i

if [[ "$i" == 'Y' || "$i" == 'y' ]]; then
    echo "YES"
else 
    echo "NO"
fi
