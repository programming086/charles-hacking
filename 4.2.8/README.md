# Usage

- Download [charles.jar](charles.jar), replace the official `charles.jar`.

- Run commands in Terminal (**For MacOS only**)

```
$ xattr Charles.app/
com.apple.quarantine
$ xattr -d com.apple.quarantine Charles.app/
$ xattr Charles.app/
```

- **Or**
- Hack with the below script by yourself.

# Hack Script

```
charles=/Applications/Charles.app/Contents/Java/charles.jar
dir=charleshack

mkdir $dir
cd $dir
cat >> qHTb.java <<EOF
package com.xk72.charles;
public final class qHTb {
    public qHTb() {}
    public static boolean DdNM() { return true; }
    public static void twLa() {}
    public static String gbef() { return "Administrator"; }
    public static String DdNM(String paramString1, String paramString2) { return null; }
}
EOF
javac -encoding UTF-8 qHTb.java -d .&& jar -uvf $charles com/xk72/charles/qHTb.class
cd .. && rm -rf $dir
```

# Official Download Link

- [Windows 64 bit](https://www.charlesproxy.com/assets/release/4.2.8/charles-proxy-4.2.8-win64.msi)
- [Windows 32 bit](https://www.charlesproxy.com/assets/release/4.2.8/charles-proxy-4.2.8-win32.msi)
- [macOS](https://www.charlesproxy.com/assets/release/4.2.8/charles-proxy-4.2.8.dmg)
- [Linux 64/32 bit](https://www.charlesproxy.com/assets/release/4.2.8/charles-proxy-4.2.8.tar.gz)
