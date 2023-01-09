# Python Practice Error-handling

- 1. Please right a Python Class with a Function to convert the log file in config/build.log into a beautiful json file like in the example below:

- @compileCommands function which needs to generate the final json looking like this:
```json
    [
        { "directory": "/home/user/llvm/build",
            "arguments": ["/usr/bin/clang++", "-Irelative", "-DSOMEDEF=With spaces, quotes and \\-es.", "-c", "-o", "file.o", "file.cc"],
            "file": "file.cc" 
        },

        { "directory": "/home/user/llvm/build",
            "command": "/usr/bin/clang++ -Irelative -DSOMEDEF=\"With spaces, quotes and \\-es.\" -c -o file.o file.cc",
            "file": "file2.cc" 
        },
        ...
    ]
```

- # Example Python Class:

```python
class CompileCommands(object):
    
    def __init__(***):
    ...
    
    def __call__(***):
    ...
    
    def readLogFile():
    ...
    
    def parseTree():
    ...
    
    def compileCommands():
    ...
    
def main():
    ...

``