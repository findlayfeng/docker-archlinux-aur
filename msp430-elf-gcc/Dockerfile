FROM fengch/archlinux-aur

RUN su docker -c 'yay -Sy --noprogressbar --needed --noconfirm msp430-elf-binutils msp430-elf-gcc-stage1 msp430-elf-newlib' &&\
    su docker -c 'yay -Rdd --noprogressbar --noconfirm msp430-elf-gcc-stage1' && \
    su docker -c 'yay -Sy --noprogressbar --needed --noconfirm msp430-elf-gcc msp430-elf-mcu' &&\
    rm -rf \
    /home/* \
    /usr/share/man/* \
    /var/cache/pacman/pkg/* \
    /var/lib/pacman/sync/* \
    /etc/pacman.d/mirrorlist.pacnew
