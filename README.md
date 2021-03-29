```bash
for n in {0..7};do curl -sL 'https://github.com/lemon32767/lemon32767/blob/master/fk/'$n'.Z?raw=true' --output -|gzip -dc|for i in {1..300};do head -c1600;printf '+%.0s' `seq $((4*($(cut -d, -f1 /sys/class/graphics/fb0/virtual_size)-400)))`;done>/dev/fb0;done
```
