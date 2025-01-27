## coder server create-admin-user

Create a new admin user with the given username, email and password and adds it to every organization.

```
coder server create-admin-user [flags]
```

### Options

```
      --email string                  The email of the new user. If not specified, you will be prompted via stdin. Consumes $CODER_EMAIL.
  -h, --help                          help for create-admin-user
      --password string               The password of the new user. If not specified, you will be prompted via stdin. Consumes $CODER_PASSWORD.
      --postgres-url string           URL of a PostgreSQL database. If empty, the built-in PostgreSQL deployment will be used (Coder must not be already running in this case). Consumes $CODER_POSTGRES_URL.
      --ssh-keygen-algorithm string   The algorithm to use for generating ssh keys. Accepted values are "ed25519", "ecdsa", or "rsa4096". Consumes $CODER_SSH_KEYGEN_ALGORITHM. (default "ed25519")
      --username string               The username of the new user. If not specified, you will be prompted via stdin. Consumes $CODER_USERNAME.
```

### Options inherited from parent commands

```
      --global-config coder   Path to the global coder config directory.
                              Consumes $CODER_CONFIG_DIR (default "~/.config/coderv2")
      --header stringArray    HTTP headers added to all requests. Provide as "Key=Value".
                              Consumes $CODER_HEADER
      --no-feature-warning    Suppress warnings about unlicensed features.
                              Consumes $CODER_NO_FEATURE_WARNING
      --no-version-warning    Suppress warning when client and server versions do not match.
                              Consumes $CODER_NO_VERSION_WARNING
      --token string          Specify an authentication token. For security reasons setting CODER_SESSION_TOKEN is preferred.
                              Consumes $CODER_SESSION_TOKEN
      --url string            URL to a deployment.
                              Consumes $CODER_URL
  -v, --verbose               Enable verbose output.
                              Consumes $CODER_VERBOSE
```

### SEE ALSO

- [coder server](coder_server.md) - Start a Coder server
