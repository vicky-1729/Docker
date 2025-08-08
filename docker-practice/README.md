# Docker-Practice

### Difference between VM vs Containers

VM(flat) 				Containers(Bed)
Costly					less cost
more time(boot time)	less time(Boot time)
more size				small size
more resources			less resources
block the resources		dynamic resources allocation
Hypervisor				no need of extra components
Not portable			Portable
More secure				Less secure(We can acheive security)

## install steps
```sudo dnf -y install dnf-plugins-core```

```sudo dnf config-manager --add-repo https://download.docker.com/linux/rhel/docker-ce.repo```

```sudo dnf install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin```

#as normal user docker cant't run we need to add your normal user to docker group
```sudo usermod -aG docker ec2-user```

