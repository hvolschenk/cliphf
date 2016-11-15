# CliPh-F
Very simple PHP CLI formatter.

## Usage

### Output

You can format output for the command line with the `Output::format` static method. It takes in only one argument and that is the string to be formatted. You can specify formats in an HTML-like syntax as in the following example:

```
Output::format('{italic}Checking config{/italic}...');
if ($something === true) {
  Output::format('{bold}{green}Done.{/green}{/bold}')
}
```

### Input

Capuring input is just as simple. You can specify normal text inputs and password inputs through CliPh-F with formatted labels:

```
$name = Input::text('Please enter your name: ');
$password = Input::password('Secret password: ');
```
