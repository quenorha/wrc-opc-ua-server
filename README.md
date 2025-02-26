# wrc-opc-ua-server

### Build
```
curl -k -o /root/build https://raw.githubusercontent.com/wrc-opc-ua-server/sssd/refs/heads/main/build && chmod +x /root/build && /root/build
```

### Run
```
docker run -d -p 54541:54541 --name wrc-opc-ua-server wrc-opc-ua-server
```

### Run with a config file
Optional, download example config file
```
curl -k -o /root/build https://raw.githubusercontent.com/wrc-opc-ua-server/sssd/refs/heads/main/project.xml
```
You can also create your config file using WRC Project Explorer
```
docker run -d -p 54541:54541 --name wrc-opc-ua-server -v /root/project.xml:/app/data/project.xml wrc-opc-ua-server
```
