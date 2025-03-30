## Create a Virtual environment so that you know what exact local dependencies the application needs 
<python -m venv test_venv> - this creates a virtual environment with the name <test_venv>
<test_venv\Scripts\activate> - to activate and enter inside the <test_venv> virtual env 
<deactivate> - deactivates the virtual environment
<pip list> - lists all the packages installed in the current environment

## Test your venv
### Step 1
Execute the below code in the global env first without and then with rich module installed
```
from rich.console import Console

console = Console()
console.print("[bold magenta]Hello, Rich![/bold magenta]")
```

### Step 2
Execute the below code in your venv, even when it is installed in global env, it will give you an error and will prompt you to install rich module. The code gets executed when you install rich module inside the venv 
```
from rich.console import Console

console = Console()
console.print("[bold magenta]Hello, Rich![/bold magenta]")
```



