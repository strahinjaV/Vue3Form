# advanced-forms

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
If you run into this error "ERR_OSSL_EVP_UNSUPPORTED" replace the "build" and "serve" scripts in the package.json file with 
"serve": "SET NODE_OPTIONS=--openssl-legacy-provider && vue-cli-service serve",
"build": "SET NODE_OPTIONS=--openssl-legacy-provider && vue-cli-service build"
then run npmm serve
```

### Compiles and minifies for production
```
npm build
```

### Lints and fixes files
```
npm lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
