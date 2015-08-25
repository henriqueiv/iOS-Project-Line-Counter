##Counting lines
This is just a list of shell scripts that count the lines of each file and shows the total number of lines at the end.

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

####In terminal
1. Open Terminal.app
2. Copy, paste and run the script that fits your need.


####On Xcode
1. Go to your project using the "Project Navigator"
2. Go to the desired target
3. Go to "Build Phases"
4. Click on the "+" sign on the left upper corner and select "New Run Script Phase"
5. Xcode will create a new entry named "Run Script"
6. Open this new script and paste the script

![Image of Xcode with custom script]
(http://i.imgur.com/9IKBoSi.png)
