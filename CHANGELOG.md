# svelte-asyncable changelog
# 2.2.0
* Bump up Svelte version in peerDeps.

# 2.1.1
* Fix repository references.

# 2.1.0
* Fix bug with error if oldValue is an error.
* Improve typings.

# 2.0.4
* Improve typings.

# 2.0.3
* Fix `syncable` bug.
* Improve typings.

# 2.0.2
* Improve typings.

# 2.0.1
* Minor fix in `package.json`.

# 2.0.0
* (breaking change): `asyncable` now is not default export.
* `syncable` store added.
* Add types.

# 1.4.1
* Add babel and prettier configs to `package.json`.

## 1.4.0
* Repository structure, code formating etc. improvements.

## 1.3.1
* Rollback a part of the previous commit. The regression test shows that we couldn't resolve a value to check it for `undefiend`. If `getter` wants to keep the current value, it should return `undefined` in an obvious way.

## 1.3.0
* Fix previous commit (forgot to resolve value before checking).
* Now bundles are also shipping.

## 1.2.0
* Now, if `getter` return `undefined` it means that store should keep current value.

## 1.1.0
* Added `svelte` as peerDependency
* Used an optimistic UI approach and set new value instantly with rollback to previous value if `setter` failed.
* Added simple check of new and old values before value update to prevent unnecessarily triggering for primitive values.

## 1.0.7

* `reducer` should receive a shallow copy of current value.

## 1.0.6

* Previous value should be resolved before passing to `setter`

## 1.0.5

* Pass previous value as a second argument of `setter`

## 1.0.4

* Perform `setter` before store update/set

## 1.0.3

* Demo example added (REPL)

## 1.0.2

* Make store read-only if `setter` is falsy

## 1.0.1

* Few optimizations

## 1.0.0

* First release
