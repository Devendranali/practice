HI this file belongs to bash scripting Repository

# #!/bin/bash
# a=5
# b=10

# if [ $a -le $b ];
# then
#     echo "$a is less than $b"
# fi


#!/bin/bash
# str1="apple"
# str2="orange"

# if [ "str1" == "str2" ];
# then
# echo "strings are equals"
# else
# echo "strings are not equals"
# fi


#!/bin/bash
# mkdir sample.txt
# file="sample.txt"
# echo $file
# if [ -e "$file" ];
# then
# echo "its a directory type"
# else
# echo "its not a directory type"
# fi


#!/bin/bash
# for i in {1..10};
# do
# tab=$((2 * $i)) 
# echo "2 * $i = $tab"
# done


#!/bin/bash
# read i
# a=1
# while [ $a -le 10 ];
# do
# table=$(($i * $a))
# echo "$i * $a = $table"
# ((a++))
# done


# #!/bin/bash
# i=1
# until [ $i -gt 5 ]; do
#     echo "Number: $i"
#     ((i++))
# done


#!/bin/bash
# echo "Hello World" > output.txt
# echo "Hello program" >> output.txt


#!/bin/bash
# touch input.txt
# echo "Hello, this is a test file, It has multiple lines." > input.txt
# cat < input.txt
# if [ -e "input.txt" ];
# then
# echo "file presents"
# else
# echo "file not presents"
# fi


#!/bin/bash
mkdir sample.txt
cd sample.txt
touch file{1..5}
ls
rm file{3..5}
ls -l
echo "this is file1" > file1
echo "this is second line in file1 " >> file1
cat<file1
rm file2
ls -l 
ls file2
echo $?
find . -name "file1"
trap "echo Goodbye!; exit" SIGINT
while true; do
    echo "Press Ctrl+C to exit."
    sleep 1
done
