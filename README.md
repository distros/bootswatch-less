# Bootswatch-less

This package contains only the less files of [bootswatch](https://github.com/thomaspark/bootswatch).
This should be used when compiling bootswatch from source using less.

Total filesize is about 600 kb.

Should be used with the [`bootstrap-less`](https://www.npmjs.com/package/bootstrap-less) package.

This package should be added to your less `paths` settings:

    gulp.pipe(less({
        paths: [
            '.',
            './node_modules/bootswatch-less'
        ]
    }))

Then bootswatch files can be included in any less file:

	@import "bootswatch/cyborg/variables";
	@import "bootswatch/cyborg/bootswatch";
