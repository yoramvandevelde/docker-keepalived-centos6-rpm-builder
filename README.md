# keepalived for CentOS6 RPM builder

Build it:
```
docker build -t keepalived-centos6-rpm-builder .
```

Run it:
```
docker run -ti --rm -v $PWD/data:/data -v $PWD/assets/config:/config keepalived-centos6-rpm-builder:latest start.sh
```

Find the RPM's in de data folder:
```
$ ls data/ 
keepalived-3.5.1-5.el6.centos.x86_64.rpm  
keepalived-debuginfo-3.5.1-5.el6.centos.x86_64.rpm
```
