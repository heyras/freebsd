# FREEBSD


# Getting your window manager installed
! and the apps you need.

```
# pkg install xorg
# pkg install dwm
# pkg install surf-browser
# pkg install password-store
# pkg install vim-lite
# pkg install tarsnap
# pkg install liberation-fonts-ttf
# pkg install sourcecodepro-ttf

# cat << EOF > /usr/local/etc/X11/xorg.conf
Section "Files"
FontPath "/usr/local/share/fonts/Liberation"
FontPath "/usr/local/share/fonts/SourceCodeProd"
EndSection
EOF

# portsnap fetch extract
# fetch http://st.suckless.org/patches/st-0.6-no-bold-colors.diff
# fetch http://st.suckless.org/patches/st-0.6-solarized-dark.diff
# cd /usr/ports/x11/sterm
# make fetch extract
# patch work/st-0.6/st.c ~/st-0.6-no-bold-colors.diff
# patch work/st-0.6/config.def.h ~/st-0.6-solarized-dark.diff
# make install 
# cd
# echo "exec dwm" > ~/.xinitrc
# startx

; once X is started, run setxkbmap dk to get the right keyboard.
```


* https://help.github.com/articles/github-flavored-markdown/
