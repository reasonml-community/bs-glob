
# bs-glob

BuckleScript bindings to [node-glob](https://github.com/isaacs/node-glob).

Status: Very basic, but functional

## Example

```ml
(* OCaml *)
Glob.glob "**/*.js" (fun _ files -> Array.iter Js.log files)
```

```reason
/* Reason */
Glob.glob("**/*.js", (_, files) => Array.iter(Js.log, files));
```

## Installation

```sh
npm install --save reasonml-community/bs-glob
```

Then add `bs-glob` to `bs-dependencies` in your `bsconfig.json`:
```js
{
  ...
  "bs-dependencies": ["bs-glob"]
}
```
