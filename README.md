# Vagrant para keywork

## Init and start

```bash
vagrant up
```

## Stop

```bash
vagrant halt
```

## Suspend

```bash
vagrant suspend
```

## Resume

```bash
vagrant resume
```

## Start

```bash
vagrant up
vagrant ssh
[ $(ifconfig eth1 | grep inet | wc -l) = 0 ] && sudo ifup eth1
docker start idm
exit
```

> Por bug del `vagrant`, forzamos el inicio de interface de red

## Stop

```bash
vagrant ssh
docker stop idm
exit
vagrant hatl
```
