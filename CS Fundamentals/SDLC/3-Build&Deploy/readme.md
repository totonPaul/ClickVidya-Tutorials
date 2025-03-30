https://pyinstaller.org/en/stable/usage.html

Create a venv and put calc.py there
### The Build Process or the Bundling Process
PyInstaller reads a Python script written by you. It analyzes your code to discover every other module and library your script needs in order to execute. Then it collects copies of all those files – including the active Python interpreter! – and puts them with your script in a single folder, or optionally in a single executable file.

You distribute the bundle as a folder or file to other people, and they can execute your program. To your users, the app is self-contained. They do not need to install any particular version of Python or any modules. They do not need to have Python installed at all.

The build folder contains a list of temporary files used to combine everything (python, your script, any other dependency) into a single .exe file, can be deleted once we have the .exe file in the dist (distribution) folder. 


If you want to run PyInstaller from Python code to build or bundle a pythin script, you can use the run function defined in PyInstaller.__main__. For instance, the following code:
```
import PyInstaller.__main__

PyInstaller.__main__.run([
    'calc.py',
    '--onefile',
    '--windowed'
])
```
Is equivalent to:

```
pyinstaller calc.py --onefile --windowed
```