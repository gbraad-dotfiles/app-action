gbraad's Dotfiles `apps` action
===============================

Use dotfiles' `apps`-command to install applications

### Usage

```yaml
      - name: Setup environment
        uses: gbraad-dotfiles/install-action@main
        
      - name: Install brew
        uses: gbraad-dotfiles/apps-action@main
        with:
          appname: brew
          command: install

      - name: Install `mc` using brew
        uses: gbraad-dotfiles/apps-action@main
        with:
          appname: mc
          command: install
          packager: brew
```

Have a look here for an [example workflows](https://github.com/gbraad-dotfiles/actions-test/blob/main/.github/workflows/test-devenv.yml).
