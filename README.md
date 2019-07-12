# platt_test
A simple layout test based off of a provided PDF layout.  

** A few items to note:** 

- The mockup provided was speced for tablet/mobile view.
- Part of the requirements called for a vanilla `CSS` with no front end layout tools.
- Features a simple `Vue` powered search tool set to query a public star wars API for character names. **For example**: `Luke` 


## Dev Environment
- node version v10.15.1

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Deploy to Github Pages:
- Create a PR for `master`
- Make sure `./deploy.sh` is executable.
- Run `$ ./deploy.sh` to compile assets and push to the `gh-pages` branch.


### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
