[![Actions Status](https://github.com/atoomic/ExtUtils-MakeMaker-PPPort/workflows/testsuite/badge.svg)](https://github.com/atoomic/ExtUtils-MakeMaker-PPPort/actions)

# SYNOPSIS

```perl
# Makefile.PL
use ExtUtils::MakeMaker::PPPort;

WriteMakefile(
  NAME           => 'Foo::Bar',
  ...
  MIN_PPPORT_VERSION => 3.58, # optional
);
```

# DESCRIPTION

This module allows you to use an up to date version of ppport.h
when using Devel-PPPort.

You do not need to ship an old version of \`ppport.h\` with your codebase.

# Migration to ExtUtils::MakeMaker::PPPort

You want to remove \`ppport.h\` from your directory and ignore it in your version control.

```
rm -f ppport.h
echo 'ppport.h' >> .gitignore
```

Then you can start using \`ExtUtils::MakeMaker::PPPort\` instead of \`ExtUtils::MakeMaker\`.

# BUGS

No known bugs.

Please report any bugs to GitHub Issues at
[https://github.com/atoomic/ExtUtils-MakeMaker-PPPort/issues](https://github.com/atoomic/ExtUtils-MakeMaker-PPPort/issues).

# SEE ALSO

[ExtUtils::MakeMaker](https://metacpan.org/pod/ExtUtils%3A%3AMakeMaker)

[Devel::PPPort](https://metacpan.org/pod/Devel%3A%3APPPort)

# SUPPORT

You can find this documentation for this module with the perldoc command.

```
perldoc ExtUtils::MakeMaker::PPPort
```

You can also look for information at:

- MetaCPAN

    [https://metacpan.org/release/ExtUtils-MakeMaker-PPPort](https://metacpan.org/release/ExtUtils-MakeMaker-PPPort)

- Github

    [https://github.com/atoomic/ExtUtils-MakeMaker-PPPort](https://github.com/atoomic/ExtUtils-MakeMaker-PPPort)

- Issues

    [https://github.com/atoomic/ExtUtils-MakeMaker-PPPort/issues](https://github.com/atoomic/ExtUtils-MakeMaker-PPPort/issues)
