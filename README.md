libSOFD - Simple Open File Dialog [for X11 without toolkit]
===========================================================

SOFD is a rather simple dialog window to allow a user to choose a file.

It is intended to be used in cross-platform toolkit-less programs (such as
audio plugins) to provide a file dialog for X11/unix systems, where other
platforms have a similar dialog from the operating system.

SOFD features:
*   single file selection
*   keyboard navigation and selection
*   "Places" list
*   "Recently used" list and API
*   plain X11 - no X extensions, no external libs, no toolkits, just 30 years too late :)

![screenshot](https://raw.github.com/x42/sofd/master/img/sofd_1.png "SOFD")

While the dialog itself is specific to the X11 Window System, the "recently
used" implementation is not and can be integrated into the application.

An example is built into the source itself. The API is documented in
the header file.

```
  gcc -Wall -D SOFD_TEST -g -o sofd libsofd.c -lX11
	./sofd
```

For a complete implementation see the source of http://xjadeo.sf.net/

libSOFD is licensed in terms of the MIT/Expat license like X11 itself.
