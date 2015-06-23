# qt5ct

qt5ct - Qt5 Configuration Tool

This program allows users to configure Qt5 settings (theme, font, icons, etc.)
under DE/WM without Qt integration.

Official home page: https://sourceforge.net/projects/qt5ct/


Requirements:

- GNU Linux or FreeBSD
- qtbase >= 5.4.0
- qtsvg >= 5.4.0 (For svg icons)
- qttools >= 5.4.0 (For build only)


Installation:

qmake PREFIX=<your installation path>
make
make install (under root)

Add line 'export QT_QPA_PLATFORMTHEME=qt5ct' to ~/.profile and re-login.

Extra build options (for advanced users only):
qmake DISABLE_WIDGETS=1 - compiles platform plugin without QtWidgets (useful only for QML applications)
qmake PLUGINDIR=<custom path> - changes a path of the platform plugin (libqt5ct.so)


Files and directories:

qt5ct - Qt5 configuration tool
libqt5ct.so - qt5ct platform plugin
~/.config/qt5ct/qt5ct.conf - configuration file
~/.config/qt5ct/qss/ - style sheets


Translation:

Use Transifex service: https://www.transifex.com/projects/p/qt5ct/
