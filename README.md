
```
beeond launch node need have ssh access to nodes
all nodes needs to resolve the beeond mgmt nodes (can be any)
beeond start -n nodefile -i /tmp/beeond.tmp -d /tmp/scratch -c /scratch -f /etc/beegfs/ -p 1999 -s $(( numnodes < 16 ? numnodes : 16 ))
beeond stop -n nodefile -i /tmp/beeond.tmp -d -L -c -q

```