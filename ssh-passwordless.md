### Generate the ssh key using ed25519
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

### Copy the public key to the remoted system
```bash
ssh-copy-id -i id_ed25519.pub user@phost
```
