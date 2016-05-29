### Generating & Adding key
Generating key:
```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

Verifing ssh-agent is running
```bash
eval "$(ssh-agent -s)"
```

Adding key to ssh-agent
```bash
ssh-add ~/.ssh/id_rsa
```

Adding new key to Git server
add the content of `id_rsa.pub` to your Git server. 
