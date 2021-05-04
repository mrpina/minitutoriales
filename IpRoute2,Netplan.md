#  IpRoute2 & NetPlan

## IpRoute2

Mostrar la ip 

- `ip addr`

Activar y desactivar interfaz de red 

- `ip link set "interface" up`
- `ip link set "interface" down`

Ejecutar dhcp interfaz

- `dhclient -v "interface"`

Establecer una nueva ip a una interfaz (se añade una ip a la interfaz aparte de la que ya tiene)

- `ip address add 192.168.x.x dev "interface"` 

Eliminar una interfaz de red 

- `ip address del 192.168.x.x dev "interface"`



## NetPlan

#### Localización del fichero

- ` /etc/netplan/*.yaml`

#### Configurar ip dinámica

```yaml
network:
  ethernets:
    "interface":
      dhcp4: true
  version: 2
```

#### Configurar ip estática 

```yaml
network:
  version: 2
  renderer: networkd
  ethernets:
    "interface":
     dhcp4: no
     addresses: [192.168.x.x/24]
     gateway4: 192.168.x.x
     nameservers:
       addresses: [8.8.8.8,8.8.4.4]
```

#### Aplicar NetPlan

- `sudo netplan apply`
