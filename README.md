# dev

###To run
```
docker run -d -p 2222:22 -v ~/.ssh/authorized_keys:/root/.ssh/host_authorized_keys jessefugitt/dev
```
###To connect with a client
```
ssh root@host-ip-address -p 2222
```

###To modify dev
```
git clone https://github.com/jessefugitt/dev.git
edit Dockerfile
docker build -t jessefugitt/dev .
```

###To generate keys
```
ssh-keygen -t rsa -C "your_email@example.com"
cat ~/.ssh/id_rsa.pub >> authorized_keys
```
