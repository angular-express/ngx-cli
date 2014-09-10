![AngularJS Express](http://i.imgur.com/nTj9QgN.png)

## Quick Start

The quickest way to initialize a new AngularJS Express application is to use the `ngx` executable as shown below:

Install the AngularJS Express CLI tool:

```bash
$ npm install -g ngx-cli
```

Initialize a new application:

```bash
$ ngx init
```

By default the [ngx-boilerplates/default](https://github.com/ngx-boilerplates/default) is installed.

To install an alternative boilerplate:

```bash
$ ngx init -b github-username/repo
```

Once you have installed an application boilerplate, you can add components:

```bash
# Add a component to handle AngularJS exceptions
$ ngx install angular-exception-handler

# Add a component with bootstrap compatible markup for a header with a navbar
$ ngx install bootstrap-header
```

This will automatically install the components in the `public/components` directory:

```bash
/public/components/angular-exception-handler
/public/components/bootstrap-header
```

If you want to install a component in a different directory, just add an additional argument:

```bash
# Install bootstrap-header component as header component
$ ngx install bootstrap-header header
```

will be installed in:

```bash
/public/components/header
```

### License
[MIT](LICENSE)