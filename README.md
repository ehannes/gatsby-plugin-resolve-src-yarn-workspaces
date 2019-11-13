This is a new gatsby site which has been moved to the `a` workspace.
I have done the following:
- Removed gatsby-plugin-manifest (since I had some building problems
  with Sharp, never mind that)
- Added the gatsby-plugin-resolve-src plugin and it's configuration in
gatsby-config
- Changed the link in src/components/layout.js to `Header` using relative path (not
  working)

Run the project with `yarn workspace a gatsby develop` and you'll get this error:
```
 ERROR #98123  WEBPACK

 Generating development JavaScript bundle failed

 Can't resolve 'components/header' in '/project-path/gatsby-resolve-src/a/src/components'

 File: src/components/layout.js

 failed Building development bundle - 2.107s
```
