# Idiomatic Javascript


These are guidelines I follow for clean, readable and performant javascript.

## You should:

+ Lint/hint your source code.
+ Minify your source code before pushing to production.
+ Keep your source code and your minified development/production code separated.
+ Use sourcemaps with your minified dev/production files to ease development.

## You should not:

+ Use any shorthand. Ever.

Why? Because shorthand code is not easily legible. It sacrifices readability to save a few bits but since you're minifying your source code, you don't need to worry about saving any bits!

+ Put all logic into one single file.

Why? Because that file is going to get difficult to maintain very quickly. Also, it's most likely that every page of your site or app doesn't need or use every single line of your js file. 

Instead, keep all site-wide functionality (navigation logic, for instance) in a single file. All other logic (page or module-specific) belongs in a separate, namespaced file (home.page.js, slideshow.module.js) to be dynamically loaded by your main file.
