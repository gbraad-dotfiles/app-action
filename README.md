gbraad's Dotfiles `apps` action
===============================

Runs `app` from my dotfiles to install applications according to the [application defintions](https://github.com/gbraad-dotfiles/applications). These are Actionfiles specifically to handle application related tasks, like installation, service install, desktop export, etc.

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
          action: install brew
```

Have a look here for an [example workflows](https://github.com/gbraad-dotfiles/actions-test/blob/main/.github/workflows/test-apps.yml).
