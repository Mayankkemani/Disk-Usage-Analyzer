
created a file disk-a.sh with the help of touch command
after that open file with text editor nano
nano disk-a.sh
after that i write bash script



***(#!/bin/bash

echo "==============================="

echo " Disk Usage Analyzer"

echo "==============================="

echo
echo "Total Disk Usage:"
df -h


echo

echo "Top 10 largest directories in current location:"

du -sh * 2>/dev/null | sort -hr | head -10


echo

echo "Top 10 largest items in /var:"

du -sh /var/* 2>/dev/null | sort -hr | head -10

echo

echo "Analysis completed.")***



AFTER that i give a permission

chmod +x disk-a.sh

than run the script

./disk-a.sh
