# RVX-Lite APK

[![CI](https://github.com/Scott-Nx/RVX-Lite-BIN/actions/workflows/ci.yml/badge.svg)](https://github.com/Scott-Nx/RVX-Lite-BIN/actions/workflows/ci.yml)

A pre-compiled binary package (apk) of ReVanced Extended (RVX) that uses a minimal set of patches.

See the [patch list](./patch-set/apply-patches.md) for details.

Get the [latest CI release](https://github.com/Scott-Nx/RVX-Lite-BIN/releases).

<details><summary><big>Features</big></summary>
<ul>
 <li>Support all present and future RVX apps</li>
 <li> Updated daily with the latest versions of apps and patches</li>
 <li> Optimize APKs and modules for size</li>

</ul>
Note that the <a href="../../actions/workflows/ci.yml">CI workflow</a> is scheduled to build the modules and APKs everyday using GitHub Actions if there is a change in RVX patches.
</details>

## To include/exclude patches or patch other apps

- Star the repo :eyes:
- Use the repo as a [template](https://github.com/new?template_name=revanced-magisk-module&template_owner=j-hc)
- Customize [`config.toml`](./config.toml) using [rvmm-config-gen](https://j-hc.github.io/rvmm-config-gen/)
- Run the build [workflow](../../actions/workflows/build.yml)
- Grab your modules and APKs from [releases](../../releases)

also see here [`CONFIG.md`](./CONFIG.md)

## Building Locally

### On Termux

```console
bash <(curl -sSf https://raw.githubusercontent.com/j-hc/revanced-magisk-module/main/build-termux.sh)
```

### On Desktop

```console
$ git clone https://github.com/j-hc/revanced-magisk-module
$ cd revanced-magisk-module
$ ./build.sh
```
