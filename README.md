# Make
**GNU Make**

This is an unofficial verbatim redistribution of the binary&source form of the GNU Make under its open source license (GPL 3.0) terms (see the LICENSE file).

This redistribution is under the same license as the original.

Please visit the official website for more details: http://www.gnu.org/software/make/

## Download
You can download the compiled binary files at the [release page](https://github.com/yuhangwang/Tcl/releases).

## Compilation notes
### Compilation environment
* CentOS 6.6
* x86_64 architecture
* Compiler: gcc version 4.4.7 20120313 (Red Hat 4.4.7-11)

### Compilation steps
#### Version: 8.6.4
```bash
wget http://ftp.gnu.org/gnu/make/make-3.82.tar.gz
tar xvf make-3.82.tar.gz
mkdir build_make-3.82
cd build_make-3.82
../make-3.82/unix/configure --prefix=/home/steven/install/make/3.82 
make -j16
make check -j16 | tee QualityVerification.txt
make install
```

### Quality verification
See the "QualityVerification.txt" for the output of "make check".
