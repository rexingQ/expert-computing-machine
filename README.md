# expert-computing-machine
5262419 1 47454e45534953 65 416672696361486f6e65 68747470733a2f2f6170692e686f6e6579706f696e74732e636173682f7370656373 0 0 2 00000000000f4240
{
  "name": "cache",
  "version": "1.1.2",
  "private": true,
  "description": "Cache dependencies and build outputs",
  "main": "dist/restore/index.js",
  "scripts": {
    "build": "tsc && ncc build -o dist/restore src/restore.ts && ncc build -o dist/save src/save.ts",
    "test": "tsc --noEmit && jest --coverage",
    "lint": "eslint **/*.ts --cache",
    "format": "prettier --write **/*.ts",
    "format-check": "prettier --check **/*.ts"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/actions/cache.git"
  },
  "keywords": [
    "actions",
    "node",
    "cache"
  ],
  "author": "GitHub",
  "license": "MIT",
  "dependencies": {
    "@actions/core": "^1.2.0",
    "@actions/exec": "^1.0.1",
    "@actions/http-client": "^1.0.6",
    "@actions/io": "^1.0.1",
    "uuid": "^11.0.5"
  },
  "devDependencies": {
    "@types/jest": "^24.0.13",
    "@types/nock": "^11.1.0",
    "@types/node": "^12.0.4",
    "@types/uuid": "^3.4.5",
    "@typescript-eslint/eslint-plugin": "^2.7.0",
    "@typescript-eslint/parser": "^2.7.0",
    "@zeit/ncc": "^0.20.5",
    "eslint": "^6.6.0",
    "eslint-config-prettier": "^6.5.0",
    "eslint-plugin-import": "^2.18.2",
    "eslint-plugin-jest": "^23.0.3",
    "eslint-plugin-prettier": "^3.1.1",
    "jest": "^24.8.0",
    "jest-circus": "^24.7.1",
    "nock": "^11.7.0",
    "prettier": "^1.19.1",
    "ts-jest": "^24.0.2",
    "typescript": "^3.7.3"
  }{
  "name": "cache",
  "version": "1.1.2",
  "private": true,
  "description": "Cache dependencies and build outputs",
  "main": "dist/restore/index.js",
  "scripts": {
    "build": "tsc && ncc build -o dist/restore src/restore.ts && ncc build -o dist/save src/save.ts",
    "test": "tsc --noEmit && jest --coverage",
    "lint": "eslint **/*.ts --cache",
    "format": "prettier --write **/*.ts",
    "format-check": "prettier --check **/*.ts"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/actions/cache.git"
  },
  "keywords": [
    "actions",
    "node",
    "cache"
  ],
  "author": "GitHub",
  "license": "MIT",
  "dependencies": {
    "@actions/core": "^1.2.0",
    "@actions/exec": "^1.0.1",
    "@actions/http-client": "^1.0.6",
    "@actions/io": "^1.0.1",
    "uuid": "^11.0.5"
  },
  "devDependencies": {
    "@types/jest": "^24.0.13",
    "@types/nock": "^11.1.0",
    "@types/node": "^12.0.4",
    "@types/uuid": "^3.4.5",
    "@typescript-eslint/eslint-plugin": "^2.7.0",
    "@typescript-eslint/parser": "^2.7.0",
    "@zeit/ncc": "^0.20.5",
    "eslint": "^6.6.0",
    "eslint-config-prettier": "^6.5.0",
    "eslint-plugin-import": "^2.18.2",
    "eslint-plugin-jest": "^23.0.3",
    "eslint-plugin-prettier": "^3.1.1",
    "jest": "^24.8.0",
    "jest-circus": "^24.7.1",
    "nock": "^11.7.0",
    "prettier": "^1.19.1",
    "ts-jest": "^24.0.2",
    "typescript": "^3.7.3"
  }
}Skip to content
Navigation Menu

Code
Issues
32
Validate 'setup-go'
Validate 'setup-go' #2443
Annotations
1 warning
oldstable (ubuntu-latest)
succeeded 1 hour ago in 12s
1s
4s
2s
Run ./
  with:
    go-version: oldstable
    check-latest: false
    token: ***
    cache: true
Setup go version spec oldstable
oldstable version resolved as 1.23.6
Found in cache @ /opt/hostedtoolcache/go/1.23.6/x64
Added go to the path
Successfully set up Go version oldstable
/opt/hostedtoolcache/go/1.23.6/x64/bin/go env GOMODCACHE
/opt/hostedtoolcache/go/1.23.6/x64/bin/go env GOCACHE
/home/runner/go/pkg/mod
/home/runner/.cache/go-build
Warning: Restore cache failed: Dependencies file is not found in /home/runner/work/setup-go/setup-go. Supported file pattern: go.sum
go version go1.23.6 linux/amd64

go env
  GO111MODULE=''
  GOARCH='amd64'
  GOBIN=''
  GOCACHE='/home/runner/.cache/go-build'
  GOENV='/home/runner/.config/go/env'
  GOEXE=''
  GOEXPERIMENT=''
  GOFLAGS=''
  GOHOSTARCH='amd64'
  GOHOSTOS='linux'
  GOINSECURE=''
  GOMODCACHE='/home/runner/go/pkg/mod'
  GONOPROXY=''
  GONOSUMDB=''
  GOOS='linux'
  GOPATH='/home/runner/go'
  GOPRIVATE=''
  GOPROXY='https://proxy.golang.org,direct'
  GOROOT='/opt/hostedtoolcache/go/1.23.6/x64'
  GOSUMDB='sum.golang.org'
  GOTMPDIR=''
  GOTOOLCHAIN='auto'
  GOTOOLDIR='/opt/hostedtoolcache/go/1.23.6/x64/pkg/tool/linux_amd64'
  GOVCS=''
  GOVERSION='go1.23.6'
  GODEBUG=''
  GOTELEMETRY='local'
  GOTELEMETRYDIR='/home/runner/.config/go/telemetry'
  GCCGO='gccgo'
  GOAMD64='v1'
  AR='ar'
  CC='gcc'
  CXX='g++'
  CGO_ENABLED='1'
  GOMOD='/dev/null'
  GOWORK=''
  CGO_CFLAGS='-O2 -g'
  CGO_CPPFLAGS=''
  CGO_CXXFLAGS='-O2 -g'
  CGO_FFLAGS='-O2 -g'
  CGO_LDFLAGS='-O2 -g'
  PKG_CONFIG='pkg-config'
  GOGCCFLAGS='-fPIC -m64 -pthread -Wl,--no-gc-sections -fmessage-length=0 -ffile-prefix-map=/tmp/go-build1076634855=/tmp/go-build -gno-record-gcc-switches'
  
0s
Run go version
  go version
  shell: /usr/bin/bash -e {0}
go version go1.23.6 linux/amd64
0s
Post job cleanup.
/opt/hostedtoolcache/go/1.23.6/x64/bin/go env GOMODCACHE
/opt/hostedtoolcache/go/1.23.6/x64/bin/go env GOCACHE
/home/runner/go/pkg/mod
/home/runner/.cache/go-build
Warning: Cache folder path is retrieved but doesn't exist on disk: /home/runner/go/pkg/mod
Primary key was not generated. Please check the log messages above for more errors or information
1s
Post job cleanup.
/usr/bin/git version
git version 2.48.1
Temporarily overriding HOME='/home/runner/work/_temp/38ccc176-dbef-4a74-8dc7-ad24fcf8bbd4' before making global git config changes
Adding repository directory to the temporary git global config as a safe directory
/usr/bin/git config --global --add safe.directory /home/runner/work/setup-go/setup-go
/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
http.https://github.com/.extraheader
/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
0s
Cleaning up orphan processes
Validate 'setup-go' · actions/setup-go@5a083d0
}