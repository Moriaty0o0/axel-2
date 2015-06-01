Axel Home:

See [http://axel.alioth.debian.org/](http://axel.alioth.debian.org/) for latest information on axel


Supported architectures
-----------------------


Should compile on any decent Linux system. Additionaly, it should compile
(and run) on BSD, Solaris, Darwin (Mac OS X) and Win32 (Cygwin) systems.

If the configure script does weird things on your system, please do warn me!
I test it on as many machines and OS'es as possible, but still anything can
go wrong.



How to install/use
------------------


Run the configure script (you can supply some options if you want, try
`./configure --help` for more info) and then run `make`. The program should
compile then. There are no special requirements for Axel. You can install
the program using `make install` or you can just run it from the current
directory. You can copy the `axelrc.example` file to `~/.axelrc` then, if you
want to change some of the settings.


Run the program like this:

```
axel ftp://ftp.nl.kernel.org/pub/linux/kernel/v2.2/linux-2.2.20.tar.bz2
```


For a simple single-server-multiple-connection download, or:

```
axel ftp://ftp.{nl,be,de}.kernel.org/pub/linux/kernel/v2.2/linux-2.2.20.tar.bz2
```

If you want to use those three servers for the download. The program can do
an automatic search for FTP mirrors as well (filesearching.com), but that's
not yet perfect... Just try the `-S` option. (The line above should at least
work with the Bash shell. You can type all the mirrors by hand as well, if
you really want to, and/or of necessary...)


Just one other thing you should keep in mind when using this program: Some
FTP operators don't like people who use download accelerators. To quote an
administrator at Progeny.Com in a mail to me:

> Additionally, I should mention that accelerated downloads are
> discouraged as I consider them abusive.

And he certainly has a point.. Using more than one server at once is a fine
solution IMHO, so please use this feature if possible!

Wilmer van der Gaast. <wilmer@gaast.net>
