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
cat >> kKPk.java <<EOF
package com.xk72.charles;
public final class kKPk {
    public kKPk() {}
    public static boolean lcJx() { return true; }
    public static void KcPF() {}
    public static String JZlU() { return "Administrator"; }
    public static String lcJx(String paramString1, String paramString2) { return null; }
}
EOF
javac -encoding UTF-8 kKPk.java -d .&& jar -uvf $charles com/xk72/charles/kKPk.class
cd .. && rm -rf $dir
```

# Official Download Link

- [Windows 64 bit](https://www.charlesproxy.com/assets/release/4.2.7/charles-proxy-4.2.7-win64.msi)
- [Windows 32 bit](https://www.charlesproxy.com/assets/release/4.2.7/charles-proxy-4.2.7-win32.msi)
- [macOS](https://www.charlesproxy.com/assets/release/4.2.7/charles-proxy-4.2.7.dmg)
- [Linux 64/32 bit](https://www.charlesproxy.com/assets/release/4.2.7/charles-proxy-4.2.7.tar.gz)
