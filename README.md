# Idiotmatic Javascript


These are guidelines I follow for clean, readable and performant javascript.

## You should:

+ Lint/hint your source code.
+ Minify your source code before pushing to production.
+ Keep your source code and your minified development/production code separated.
+ Use sourcemaps with your minified dev/production files to ease development.

## You should not:

+ Use any shorthand. Ever.

Why? Because shorthand code is not easily legible. It sacrifices readability to save a few bits but since you're minifying your source code, you don't need to worry about saving any bits!


