![angular-express-header](https://cloud.githubusercontent.com/assets/1859381/8266502/d94e93ce-1731-11e5-9b9d-9b9e58c5369f.png)

Command line tool for [AngularJS Express](http://www.angular-express.com).

## Installation

```bash
$ npm install -g ngx-cli
```

## ngx init

Initialize a boilerplate to kickstart a project:

```bash
$ ngx init [options] [target-directory]
```

#### Options

##### `-b, --boilerplate <boilerplate>`

Boilerplate to initialize.
 
Format: `[<github-username>/]<github-repository-name>`.

- if no boilerplate is specified, `ngx-boilerplates/default` is used
- if only a `<github-repository-name>` is specified, `ngx-boilerplates/<github-repository-name>` is used

##### `-f, --force`

Overwrite existing file(s).

##### `-h, --help`

Output usage information.

#### Arguments

##### `<target-directory>`

Where to initialize the boilerplate.

- if no `target-directory` is specified, the current directory is used

#### Examples:

```bash
# Initialize ngx-boilerplates/default in current directory
$ ngx init

# Initialize ngx-boilerplates/default in directory new-project
$ ngx init new-project

# Initialize ngx-boilerplates/default in current directory
$ ngx init -b default

# Initialize github-username/github-repository-name in current directory
$ ngx init -b github-username/github-repository-name
```

Visit [ngx-boilerplates](https://github.com/ngx-boilerplates) for a list of official boilerplates.

## ngx install

Install a component in an existing project:

```bash
$ ngx install [options] <component> [target-directory]
```

#### Options

##### `-f, --force`

Overwrite existing file(s).

##### `-h, --help`

Output usage information.

#### Arguments

##### `<component>`

Component to install.
 
Format: `[<github-username>/]<github-repository-name>`

- if only a `<github-repository-name>` is specified, `ngx-components/<github-repository-name>` is used

##### `<target-directory>`

Where to install the component.

- if no `target-directory` is specified, `src/components` is used

#### Examples:

```bash
# Install ngx-components/angular-ui-router-component in src/components/angular-ui-router-component
$ ngx install angular-ui-router-component

# Install ngx-components/angular-ui-router-component in src/components/homepage
$ ngx install angular-ui-router-component src/components/homepage

# Install github-username/foo in src/components/foo
$ ngx install github-username/foo

# Install github-username/foo in src/components/bar
$ ngx install github-username/foo in src/components/bar
```

Visit [ngx-components](https://github.com/ngx-components) for a list of official components.

### License
[MIT](LICENSE)

### Change log

### v1.4.0

- Removed Harp dependency
- Removed compile command
- Updated documentation

### v1.2.0

- Added compile command
- Updated documentation

### v1.0.0

- Added support for installing components in `src/components` by default
- Updated documentation

### v0.1.0

- Initial version
