# Ubuntu instal
# Zmiana adresu IP na atayczny w karcie sieciowej

'sudo vim /etc/netplan/00-installer-config.yaml'

# Zawartosc pliku konfiguracyjnego stale ip
'
# This is the network config written by 'subiquity'
network:
  version: 2
  renderer: networkd
  ethernets:
    enp1s0:
      dhcp4: true
      addresses: [192.168.3.223/24]
      gateway4: 192.168.3.1
      nameservers:
        addresses: [192.168.0.1,8.8.8.8]
        '


# Sprawdzanie jakie sa pliki w katalogu

'sudo ls /etc/netplan/ '

# Sprawdzanie jakie karty sieciowe 

'sudo ifconfig -a'

