# SublimeCodeFormatter
This plugins enables you to format code using an external tool.

# Usage
To add a formatter to the plugin you have to add it to the preferences.
For example, to use clang-format to format c language files and autopep8 
for python files add the following:
```json
{
	"formatters": {
    		"c": "clang-format -arg1 -arg2 -arg3",
    		"python": "autopep8"
    	}
    },
    "format_on_save" : true,
}
```
Also note that `format_on_save` is disabled by default. In the example
above it is now enabled.

Now it is possible to use `CTRL+SHIFT+Q` (or `SUPER+SHIFT+Q` on OS X) to
format an open `.c` file, or just save to format the file.
