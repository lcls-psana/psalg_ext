# psalg_ext
This package is required to build *external* psalg package.

## Quick start
### Create conda release
See [Psana Developer Documentation](https://confluence.slac.stanford.edu/display/PSDMInternal/Psana+Developer+Documentation)
```
cd <my-conda-release>
source conda_setup
```

### Clone packages
**on pslogin:**

Add psalg_ext
```
git clone https://github.com/lcls-psana/psalg_ext.git
# or 
condarel --addpkg --name psalg_ext --tag HEAD
```
Add psalg from different repo of external packages
```
condarel --addpkg --name psalg --tag HEAD
```
### Build 
```
scons
```
### Re-build
```
rm -rf arch
scons
```
