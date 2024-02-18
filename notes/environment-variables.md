# SSH, Secret Keys, Environment Variables

This is a repository containing confidential information such as API keys.

## Custom Environment Variables

To manage our secret keys, we will locally store them in `~/.secrets` folder.

Edit .bash_profile to globally set environment variables:
```
# custom environment variables
export NAME="John Doe"
export ADDRESS="123 Main St"
export EMAIL="john@example.com"
export API_KEY="your_api_key"
export PASSWORD="your_password"
GOOGLE_APPLICATION_CREDENTIALS="/c/Users/adval/.ssh/advalen-de-zoomcamp-2024-93ebc31fb43b.json"
# End custom environment variables
```

```
# custom functions
print_custom_env() {
sed -n '/# Custom environment variables/,/# End custom environment variables/p' ~/.bash_profile
}
# end custom functions
```

## SSH Configurations
```
Host vm-dezoomcamp
    HostName 00.000.000.000
    User username
    IdentityFile /C/path-to-ssh-keys/private-key
```

```
Host hadoopcluster 
  HostName 54.85.143.224
  User hirwuser3094
  PubkeyAcceptedKeyTypes=+ssh-rsa
  IdentityFile /C/Users/adval/.ssh/hirwuser3094.pem
```