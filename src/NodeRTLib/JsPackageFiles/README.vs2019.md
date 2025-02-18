{PackageName}
=====

## Notice

The series of `@:::org:::` packages is unofficially-published NodeRT modules for **Windows :::win-major::: SDK, version :::win-minor::: (10.0.:::target-build-ver:::.0)** corresponding to Windows :::target-ver::: (:::win-desc:::).

These are generated by the modified version of NodeRT thus are experimental, as the original doesn't have support for :::win-minor::: SDK, nor for building with VS2019. Supporting for VS2019 is based on <a href="https://github.com/NodeRT/NodeRT/pull/136" target="_blank">Taosenai's workaround with lxbndr's suggestion</a>. The modified source code can be found <a href="https://github.com/MaySoMusician/NodeRT/tree/feature/136-vs2019" target="_blank">here</a>.

Below is the original description about this module.

---

A Node.js wrapper for the <a href="http://msdn.microsoft.com/en-us/library/windows/apps/{Namespace}.aspx" target="_blank">{Namespace}</a> WinRT namespace, compatible with Windows {WinVersion} APIs.

Using this module, you'll be able to consume the <a href="http://msdn.microsoft.com/en-us/library/windows/apps/{Namespace}.aspx" target="_blank">{Namespace}</a> API directly from Node.js.

This module was automatically generated by <a href="https://github.com/NodeRT/NodeRT" target="_blank">NodeRT</a>. 
For more information on NodeRT and examples on how to use NodeRT modules, please visit the project page at: <a href="https://github.com/NodeRT/NodeRT" target="_blank">https://github.com/NodeRT/NodeRT</a>.

The API exposed by this module is (almost) the same as the API that is listed in: <a href="http://msdn.microsoft.com/en-us/library/windows/apps/{Namespace}.aspx" target="_blank">http://msdn.microsoft.com/en-us/library/windows/apps/{Namespace}.aspx</a>

The only difference in the API is in the way that asynchronous methods and events are used. (See <a href="https://github.com/NodeRT/NodeRT#ConsumingNodeRT" target="_blank">https://github.com/NodeRT/NodeRT#ConsumingNodeRT</a> for more details)

This module also contains TypeScript definition files for the API exposed by the module, as well as JavaScript intellisense support for <a href="http://nodejstools.codeplex.com/" target="_blank">Node.js tools for Visual Studio</a>.

Prequisites:
============
* Visual Studio 2019 and above. (Community edition works, other editions aren't tested but surely work!)
* Python 2.7, 3.5, 3.6, 3.7, or 3.8 (for node-gyp)
* <b>Important:</b> Updated versions of npm and node-gyp. (Note that the ones that are bundled with node might not be up to date). In order to install latest npm, run:
```
npm install -g npm
```

In order to install latest node-gyp run:
```
npm install -g node-gyp
```

Installation:
=============
In order to install this module, run npm install:

```
npm install {PackageName}
```

If you wish to rebuild this module using node-gyp, make sure to use the appropriate VS version using --msvs_version=2012/2013/2015/2017/2019 flag:

For example:

```
cd [module folder path]
node-gyp rebuild --msvs_version=2019
```

If you fail to rebuild due to unable to find module 'nan', try running `npm install --ignore-scripts`