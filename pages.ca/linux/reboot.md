# reboot

> Reinicia la màquina.
> Més informació: <https://manned.org/reboot.8>.

- Reinicia inmediatament:

`reboot`

- Apaga el sistema (el mateix que `poweroff`):

`reboot {{[-p|--poweroff]}}`

- Atura el sistema (el mateix que halt):

`reboot --halt`

- Reinicia inmediatament sense contactar l'adminstrador del sistema:

`reboot {{[-f|--force]}}`

- Escriu l'entrada wtmp shutdown sense reiniciar el sistema:

`reboot {{[-w|--wtmp-only]}}`
