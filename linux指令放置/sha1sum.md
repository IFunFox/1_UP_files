# sha1sum (160bit) 不安全
---
    gedit test.txt
    測試
    sha1sum test.txt
    f6b0675405c260f5fd03c3a7846e7e6429db953e  test.txt
---
# sha224sum (224bit) 不安全
---
    測試
    9bab87f131d4fc9544936e44d5aba02af42ee3bd1fc662ee95cf9261  test.txt
---
# sha256sum (256bit) 不安全
---
    sha256sum test.txt 
    6b642ce34939923db09ff73c5dc5601d866bb62bdcc44ca8249d89f076cdbc5d  test.txt
---

# sha1sum --help
---
sha1sum --help 
Usage: sha1sum [OPTION]... [FILE]...
Print or check SHA1 (160-bit) checksums.

With no FILE, or when FILE is -, read standard input.

  -b, --binary         read in binary mode
  -c, --check          read SHA1 sums from the FILEs and check them
      --tag            create a BSD-style checksum
  -t, --text           read in text mode (default)
  -z, --zero           end each output line with NUL, not newline,
                       and disable file name escaping

The following five options are useful only when verifying checksums:
      --ignore-missing  don't fail or report status for missing files
      --quiet          don't print OK for each successfully verified file
      --status         don't output anything, status code shows success
      --strict         exit non-zero for improperly formatted checksum lines
  -w, --warn           warn about improperly formatted checksum lines

      --help     display this help and exit
      --version  output version information and exit

The sums are computed as described in FIPS-180-1.  When checking, the input
should be a former output of this program.  The default mode is to print a
line with checksum, a space, a character indicating input mode ('*' for binary,
' ' for text or where binary is insignificant), and name for each FILE.

GNU coreutils online help: <https://www.gnu.org/software/coreutils/>
Full documentation at: <https://www.gnu.org/software/coreutils/sha1sum>
or available locally via: info '(coreutils) sha1sum invocation'
---
