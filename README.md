StJetMakerTree
==============

Jet analysis tools used for the STAR experiment


### How to download, compile, and install

Befor installing this librarly, you need to install https://github.com/TaiSakuma/StJetFinder.

Checkout

    git clone git@github.com:TaiSakuma/StJetMakerTree.git
    cd StJetFinder

Run Autotools

    aclocal -I ./m4
    glibtoolize --copy --force
    autoconf
    automake --add-missing --copy --foreign

Configure (replace PREFIX with the path to which you want to install files, e.g., $HOME)

    ./configure --prefix=PREFIX

If you use a different PREFIX from the one used for StJetFinder, you might need to speficy the path to StJetFinder with CPPFLAGS.

Compile

    make

Install

    make install

this will install files in PREFIX/include and PREFIX/lib
