# vim-lsp-typescript

Sets up [vim-lsp](https://github.com/prabirshrestha/vim-lsp) for TypeScript.

_Note: This plugin no longer sets things up for JavaScript anymore. Please use [ryanolsonx/vim-lsp-javascript](https://github.com/ryanolsonx/vim-lsp-javascript) to set up `vim-lsp` for JavaScript use._

## Installing

Install typescript language server using [npm](https://www.npmjs.com):

```
npm install -g typescript typescript-language-server
```

Install the vim plugins:

```viml
" Dependencies
Plug 'prabirshrestha/async.vim'
Plug 'prabirshrestha/vim-lsp'

Plug 'ryanolsonx/vim-lsp-typescript'
```

## Usage

You must have a tsconfig.json at the root of your project and this plugin will be able to pick it up and provide TypeScript support.

## Have an Issue?

Try to reproduce with a minimal vimrc configuration. You can use the one included in this project to create a temp vim setup.

```
curl https://raw.githubusercontent.com/ryanolsonx/vim-lsp-typescript/master/minimal.vimrc -o /tmp/minimal.vimrc
vim -u /tmp/minimal.vimrc +PlugInstall +qall
vim -u /tmp/minimal.vimrc ./your_test_file.ts
```

## License

MIT
