[![AngularJS Express](http://i.imgur.com/nTj9QgN.png)](https://github.com/angular-express/angular-express)

Command line tool for [AngularJS Express](https://github.com/angular-express/angular-express).

## Installation

```bash
$ npm install -g ngx-cli
```

## ngx init

To initialize the [default boilerplate](https://github.com/ngx-boilerplates/default) from [ngx-boilerplates](https://github.com/ngx-boilerplates).

```bash
$ ngx init
```

To initialize a different boilerplate from [ngx-boilerplates](https://github.com/ngx-boilerplates):

```bash
$ ngx init -b <boilerplate-name>
```

To initialize a custom boilerplate:

```bash
$ ngx init -b <github-username/github-repository-name>
```

So:

```bash
$ ngx init
```

is the same as:

```bash
$ ngx init -b default
```

is the same as:

```bash
$ ngx init -b ngx-boilerplates/default
```

Visit [ngx-boilerplates](https://github.com/ngx-boilerplates) to view the available boilerplates.

## ngx install

To install components from [ngx-components](https://github.com/ngx-components):

```bash
# Install AngularJS exception handler component
$ ngx install angular-exception-handler

# Install Bootstrap header component
$ ngx install bootstrap-header
```

Components are automatically installed in the `src/components` directory:

```bash
# To install boostrap-header in src/components/bootstrap-header
$ ngx install bootstrap-header
```

To install a component in a different directory, just specify the destination as an additional argument:

```bash
# To install boostrap-header in src/components/header
$ ngx install bootstrap-header src/components/header
```

Specify a GitHub repository to install a custom component:

```bash
# Install a component from any GitHub repository
$ ngx install <github-username/github-repository-name>
```

If no `github-username` is specified, it defaults to `ngx-components`, so:

```bash
$ ngx install angular-exception-handler
```

is the same as:

```bash
$ ngx install ngx-components/angular-exception-handler
```

Visit [ngx-components](https://github.com/ngx-components) to view the available components.

### License
[MIT](LICENSE)

### Change log

### v1.0.0

- Added support for installing components in `src/components` by default
- Updated documentation

### v0.1.0

- Initial version
