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

## Restore

```bash
vagrant resume
```

## Restart

```bash
vagrant up
vagrant ssh
[ $(ifconfig eth1 | grep inet | wc -l) = 0 ] && sudo ifup eth1
docker start idm
exit
```

## Stop

```bash
vagrant ssh
docker stop idm
exit
vagrant hatl
```
