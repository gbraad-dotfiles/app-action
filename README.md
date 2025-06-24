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
          action: install

      - name: Install `mc` using brew
        uses: gbraad-dotfiles/apps-action@main
        with:
          appname: mc
          action: install
          packager: brew
```

Have a look here for an [example workflows](https://github.com/gbraad-dotfiles/actions-test/blob/main/.github/workflows/test-apps.yml).

Application defintions can be found in [this repository](https://github.com/gbraad-dotfiles/applications/)
.
