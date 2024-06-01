## Makefile

### Variables
- `JC`: Java compiler command (`javac`)
- `JV`: Java virtual machine command (`java`)
- `CP`: Classpath for compilation and execution, including required JAR files
- `JAVAFLAGS`: Java flags for execution
- `JCFLAGS`: Java compiler flags

### Targets
- `all`: Builds both `Example` and `GpsGui`
- `GpsGui`: Builds the `GpsGui` application
- `Example`: Builds the `Example` application
- `run`: Builds and runs both `Example` and `GpsGui`
- `gui`: Runs the `GpsGui` application
- `exp`: Runs the `Example` application
- `clean`: Removes compiled `.class` files

### How to Use

#### Compilation
To compile the Java source files and generate the executable classes, run the following command:
```bash
make all
```

#### Run All
To compile and run both `Example` and `GpsGui`, use:
```bash
make run
```

#### Run GpsGui
To run only the `GpsGui` application, use:
```bash
make gui
```

#### Run Example
To run only the `Example` application, use:
```bash
make exp
```

#### Clean
To remove all compiled `.class` files, use:
```bash
make clean
```