# omp-bsod

oh-my-posh theme - BSOD

## oh-my-posh install and config

This theme has been built for [oh-my-posh](https://ohmyposh.dev/). To install and configure with my settings:

- Open PowerShell.
- Install posh-git module `Install-Module posh-git`
- Install git `winget install git.git`
- Install gsudo `winget install gerardog.gsudo`
- Install oh-my-posh `winget install JanDeDobbeleer.OhMyPosh`
- Install the FiraCode Nerd Font with `sudo oh-my-posh font install`
- Add the following to the PS profile (`code $PROFILE`):
```Powershell
Import-Module posh-git
oh-my-posh init pwsh --config 'https://raw.githubusercontent.com/danstis/omp-bsod/main/bsod.omp.json' | Invoke-Expression
$env:POSH_AZURE_ENABLED = $true
```