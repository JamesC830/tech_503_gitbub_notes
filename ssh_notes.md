# SSH notes

### Removing SSH keys

```rm ~/.ssh/key_name```

or

```rm key_name``` 

if you are already in the .ssh directory

### Making keys

```ssh-keygen -t rsa -b 4096 -C "email"```

Generates a key

- rsa = encryption method
- 4096 = size (number of bytes)

Leave passphrase blank

```cat keyname.pub```

Gives output of the key

## Warning! Only use this on the .pub key

Paste the output into the github SSH keys section

Then do the following steps

```eval `ssh-agent -s` ```

```ssh-add keyname```

```ssh -T git@github.com```

Creates a connection with github