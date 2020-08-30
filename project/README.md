Write a small script that will take 3 parameters in any order. -A 100 -B 110 -C 120. It can also come as -C 120 -A 100 -C 110. You should check for all parameters and print error if missing. Setup github gist or repo


#!/bin/bash

echo  $1 $2 $3

if [$# -ne 3 ];then
echo "Error,not required parameters given"
else
args=("$@")
echo ${args[0]} ${args[1]} ${args[2]}
fi
