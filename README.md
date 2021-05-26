# Bootstrap4 Datetimepicker

A date/time picker component designed to work with Bootstrap 4 and Momentjs.

This is a fork of the excellent but discontinued [tempusdominus/bootstrap-4](https://github.com/tempusdominus/bootstrap-4).

The goal is to mantain it with comunity help by applying small improvements and bug fixes since we need the component for professional projects.

# Project status

I just started organizing the project. **Please do not try to use this yet**.

# Todo

-  [x] ✅ Take a look and merge PRs from [tempusdominus/bootstrap-4](https://github.com/tempusdominus/bootstrap-4) in this repo.
   -  Weird. These PR seems to already be applied although they are open:
      -  332 (minification of CSS)
      -  331 (fix for blanking cursor when clicking day on calendar)
      -  329 (Multidate mode fixes)
-  [ ] Setup github page with demos. Done: https://ww9.github.io/bootstrap4-datetimepicker/
-  [x] ✅ Update package.json with new info and package name.
-  [ ] Document usage here on README.
-  [ ] Setup npm package.
-  [ ] Switch from discontinued [momment.js](https://momentjs.com/docs/#/-project-status/) to another date library. Perhaps [Day,js](https://github.com/iamkun/dayjs)?
-  [ ] Setup CDN so people can use it easily.
-  [ ] Attempt to remove dependency on Grunt. Can we build minified js and css simply with npm scripts?
-  [ ] Also try to simplify stuff. Move docs/index.html to /index.html
   -  We don't really need mkDocs. Build all documentation and demo on a single .html file. See this about HTML code escaping: https://stackoverflow.com/a/2820460/267847
   -  Delete /docs and change github settings to point docs to main branch root
-  [ ] Remove as many dependencies as possible
-  [ ] Cleanup and change theme of documentation github page.
-  [ ] Take a look at the dependencies section in `package.json` and try to cleanup. Specially understand if this needs `tempusdominus/core`. If so, copy that lib inside this to simplify building and keep the projects independent otherwise remove the dependency (https://nodejs.org/es/blog/npm/peer-dependencies/):

```
	"dependencies": {
		"bootstrap": "^4.5.2",
		"jquery": "^3.5.1",
		"moment": "^2.29.0",
		"moment-timezone": "^0.5.31",
		"popper.js": "^1.16.1"
	},
	"peerDependencies": {
		"bootstrap": ">=4.5.2",
		"jquery": "^3.5.1",
		"popper.js": "^1.16.1",
		"moment": "^2.29.0",
		"moment-timezone": "^0.5.31",
		"tempusdominus-core": "5.19.0"
	},
```

-  [ ] Setup new jsfiddle and update docs.
-  [ ] Test with various browsers and generate browser support matrix image. Put image here on README.

# Requirements

-  jQuery
-  Bootstrap 4
-  momment.js

# Installation

-  Make sure you have the requirements. Then include these two files on your page:
   -  https://github.com/ww9/bootstrap4-datetimepicker/blob/main/build/tempusdominus-bootstrap-4.min.css
   -  https://github.com/ww9/bootstrap4-datetimepicker/blob/main/build/tempusdominus-bootstrap-4.min.js

I'll setup Github pages when I have the time.

# Credits

This package is a fork of the excellent but discontinued [tempusdominus/bootstrap-4](https://github.com/tempusdominus/bootstrap-4) repo.

# License

MIT. Feel free to use for personal and comercial.

## Submitting Issues

If you have issues, please check the following first:

-  Have you read the docs?
-  Do you have the latest version of momentjs?
-  Do you have the latest version of jQuery?
-  Please test and/or fork [this jsfiddle](https://jsfiddle.net/Eonasdan/bdxss6m8/) with an example of your issue before you post an issue here.
-  Please indicate which version of the picker you are using (this can be found at the top of any included file)
