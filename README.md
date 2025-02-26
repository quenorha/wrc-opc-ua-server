# wrc-opc-ua-server

### Build
```
curl -k -o /root/build https://raw.githubusercontent.com/wrc-opc-ua-server/refs/heads/main/build && chmod +x /root/build && /root/build
```

### Run
```
docker run -d -p 54541:54541 --name wrc-opc-ua-server wrc-opc-ua-server
```

### Run with a config file

Create your config file using WRC Project Explorer.

Optionally, download example config file
```
curl -k -o /root/build https://raw.githubusercontent.com/wrc-opc-ua-server/refs/heads/main/project.xml
```

```
docker run -d -p 54541:54541 --name wrc-opc-ua-server -v /root/project.xml:/app/data/project.xml wrc-opc-ua-server
```
