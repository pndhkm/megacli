# a) Megacli64

## Requirements
```
apt update
apt install libncurses5 alien

```

## Download
```
curl -LO https://docs.broadcom.com/docs-and-downloads/raid-controllers/raid-controllers-common-files/8-07-14_MegaCLI.zip
```

## Unzip
```
unzip 8-07-14_MegaCLI.zip
```

## Convert to debian package
```
cd Linux
alien MegaCli-8.07.14-1.noarch.rpm
```

## Installing
```
dpkg -i megacli_8.07.14-2_all.deb
```

## Link megacli to Application/distribution
```
ln -s /opt/MegaRAID/MegaCli/MegaCli64 /usr/bin/megacli
```

## Run
```
megacli -h
```

# b) Megaclisas-status for debian
## Add repo
```
deb http://mirror.rackspace.com/hwraid.le-vert.net/debian/ jessie main
```
## Update repo & install megaclisas-status
```
apt update  && apt install ## Run -y
```

## Run
```
megaclisas-status
```
