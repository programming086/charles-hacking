# Usage

- Download [charles.jar](charles.jar), replace the official `charles.jar`.
- **Or**
- Hack with the below script by yourself.

# Hack Script

```
charles=/Applications/Charles.app/Contents/Java/charles.jar
dir=charleshack

mkdir $dir
cd $dir
cat >> GPSz.java <<EOF
package com.xk72.charles;
public final class GPSz {
    public static boolean Dgmx() { return true; }
    public static void fxWP() {}
    public static String Wmmw() { return "Administrator"; }
    public static String Dgmx(String paramString1, String paramString2) { return null; }
}
EOF
javac -encoding UTF-8 GPSz.java -d .&& jar -uvf $charles com/xk72/charles/GPSz.class
cd .. && rm -rf $dir
```

# Official Download Link

- [Windows 64 bit](https://www.charlesproxy.com/assets/release/4.2.6/charles-proxy-4.2.6-win64.msi)
- [Windows 32 bit](https://www.charlesproxy.com/assets/release/4.2.6/charles-proxy-4.2.6-win32.msi)
- [macOS](https://www.charlesproxy.com/assets/release/4.2.6/charles-proxy-4.2.6.dmg)
- [Linux 64/32 bit](https://www.charlesproxy.com/assets/release/4.2.6/charles-proxy-4.2.6.tar.gz)
