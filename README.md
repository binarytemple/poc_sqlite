# poc_sqlite

This project is going to contain some sqlite experiments, also worth looking at 

Inspiration/reference for project bootstrap :  

* [Creating an open source program in c with autotools part 1 of 2](http://blog.fourthbit.com/2013/06/18/creating-an-open-source-program-in-c-with-autotools-part-1-of-2)
* [Creating an open source project in c with autotools part 2 of 2](http://blog.fourthbit.com/2013/08/05/creating-an-open-source-project-in-c-with-autotools-part-2-of-2)


I've completed that setup as far as 'adding debug support'

# setup 

OSX 
```
brew install autoconf && brew install automake
```

Clear out any non-git build artefacts
```
./purge
```

Configure, build and execute
```
autoreconf -iv && ./configure --enable-debug && make && ./src/bin/pocsqlite
```

# Build 

From a fresh copy, run :

autoreconf -iv


