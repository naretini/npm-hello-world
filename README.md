# Basics on How to publish packages to npm

- create a npm account and login
```bash
npm login
unsername: pippo
```
- create npm project:
```bash
  mkdir npm-hello-world && cd $_
  npm init --scope=pippo
```

- publish to npm (publicly):
 
[ If your repository has a scope, you need to adjust the publish command ]
```bash
 npm publish --access public
```

- create a repo on github and link to it:
```bash
   git init
   git remote add origin git@github.com:naretini/npm-hello-world.git
```


### Best practice before (npm) publish:

 - Run tests (if there are any)
 - Update version in package.json according to Semver
 - Create a git tag according to Semver
 - Push the package to Github
 - Push the package to npm
 - Create release notes for every update

 