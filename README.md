# Lens "Deployment Image Update" Extension

Lens extension to simplify update of deployment image tag:

* Just open deployment details and save new image tag.

![Image details in deployment overview](imgs/tag.png)

## Download .tgz

### Github 
https://github.com/ottimis/lens-version-update/releases/latest

### NPM

https://registry.npmjs.org/@ottimis/lens-version-update/-/lens-version-update-$VERSION.tgz

Replace `$VERSION` with a real version like `0.0.3`.


## Install

```sh
mkdir -p ~/.k8slens/extensions
git clone https://github.com/ottimis/lens-version-update.git
ln -s $(pwd)/lens-version-update ~/.k8slens/extensions/lens-version-update
```

## Build

To build the extension you can run the `npm` commands manually:

```sh
cd lens-version-update
npm install
npm run build
```

If you want to watch for any source code changes and automatically rebuild the extension you can use:

```sh
cd lens-version-update
npm start
```

## Test

Open Lens application and navigate to a cluster. You should see "Hello World" in a menu.

## Uninstall

```sh
rm ~/.k8slens/extensions/lens-version-update
```

Restart Lens application.
