# [how to install tfjs-node](https://github.com/jaaleng/gitblog/issues/12)

hey guys i need to install the tf.js server version (node), however i got some problem as this:  PS C:\WINDOWS\system32> node C:\Users\SHIIIIIISH\Desktop\dune\nu.js
node:internal/modules/cjs/loader:1460
  return process.dlopen(module, path.toNamespacedPath(filename));
                 ^

Error: The specified module could not be found.
\\?\C:\Users\SHIIIIIISH\Desktop\dune\node_modules\@tensorflow\tfjs-node\lib\napi-v8\tfjs_binding.node
    at Module._extensions..node (node:internal/modules/cjs/loader:1460:18)
    at Module.load (node:internal/modules/cjs/loader:1203:32)
    at Module._load (node:internal/modules/cjs/loader:1019:12)
    at Module.require (node:internal/modules/cjs/loader:1231:19)
    at require (node:internal/modules/helpers:177:18)
    at Object.<anonymous> (C:\Users\SHIIIIIISH\Desktop\dune\node_modules\@tensorflow\tfjs-node\dist\index.js:72:16)
    at Module._compile (node:internal/modules/cjs/loader:1364:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1422:10)
    at Module.load (node:internal/modules/cjs/loader:1203:32)
    at Module._load (node:internal/modules/cjs/loader:1019:12) {
  code: 'ERR_DLOPEN_FAILED'
}

Node.js v18.20.2
PS C:\WINDOWS\system32>

btw: windows 11 x64, py vers: Python 3.12.3. c++ tools also are here 