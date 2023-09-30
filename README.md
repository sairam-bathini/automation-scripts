#!/bin/bash

###########
#Author: Sairam Bathini
#Date: 30-09-2023
#Version: v1
#This script is used to print the type of the triangle based on the sides comparison
###########


read -p "enter the side 1" a #reading the inpout from STDIN
read -p "enter the side 2" b #reading the inpout from STDIN
read -p "enter the side 3" c #reading the inpout from STDIN

if (($a==$b)) && (($a==$c)) #checking if all three sides are equal
then echo "EQUILATERAL"
elif (($a==$b)) || (($a==$c)) || (($b==$c)) #checking if any two sides are equal
then echo "ISOSCELES"
else echo "SCALENE"
fi

