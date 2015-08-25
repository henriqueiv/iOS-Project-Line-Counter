##Counting lines
This is just a list of shell scripts that count the lines of each file and the total number of lines at the end.

####For Swift only
```
find . \( -iname \*.swift \) -exec wc -l '{}' \+
```

####For Obj-C only
```
find . \( -iname \*.m -o -iname \*.mm -o -iname \*.h \) -exec wc -l '{}' \+
```

####For Obj-C + Swift
```
find . \( -iname \*.m -o -iname \*.mm -o -iname \*.h -o -iname \*.swift \) -exec wc -l '{}' \+
```

####For Obj-C + Swift + C + C++
```
find . \( -iname \*.m -o -iname \*.mm -o -iname \*.c -o -iname \*.cc -o -iname \*.h -o -iname \*.hh -o -iname \*.hpp -o -iname \*.cpp -o -iname \*.swift \) -exec wc -l '{}' \+
```

##How to use
1. Open Terminal.app
2. Copy, paste and run the script that fits your need.
