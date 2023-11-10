# HW8
HW8 Linux

#!/bin/bash

directory=$1

for i in $(find $directory -name '*.bak' -or -name '*.tmp' -or -name '*.backup')
do
        rm "$i"
done

