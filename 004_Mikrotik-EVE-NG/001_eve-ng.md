# Dicas-Mikrotik-EVE-NG

Fontes:
<https://youtu.be/cj3qsNsBd2A>
<https://www.redesbrasil.com/aprenda-a-instalar-e-usar-o-eve-ng-para-emular-roteadores-da-mikrotik/>

Acesso web:
```
admin
```

```
eve
```

Acesso SSH:
```
root
```

```
eve
```

## 
```
mkdir -p /opt/unetlab/addons/qemu/mikrotik-6.47.10
```

```
cd /opt/unetlab/addons/qemu/mikrotik-6.47.10
```

```
wget https://download.mikrotik.com/routeros/6.47.10/chr-6.47.10.vmdk
```

```
/opt/qemu/bin/qemu-img convert -f vmdk -O qcow2 chr-6.47.10.vmdk hda.qcow2
```

```
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

```
rm -rf chr-6.47.10.vmdk
```