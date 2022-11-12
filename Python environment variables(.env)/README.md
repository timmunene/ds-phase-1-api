# python-dotenv

This is a python package that is used to read key-value pairs from a `.env` file and can set them as environment variable. 
It helps in the development of applications and programs following the [12-factor](http://12factor.net/).

## Install the python-dotenv package
```
pip install python-dotenv
```

## Environment Variable
Refers to variable comprising of key-value pairs for the current user environment stored outside the program/application through functionality built into the operating system.

### Create a `.env` file

Name the file just `.env` and *not* `~~file.env~~`.

You can now add `key=value` pairs inside the `.env` file.

📝 Avoid whitespaces before or after the `=` and putting the key or value in `""` strings.

The following is an example of the contents of a `.env` file:

```
Password=Moringa@123
ACCESS_TOKEN="ABCMoringasupersecret123XYZ"
```

A variable's value can be used again within the same file using `${var}`.

```
PATH=moringa/credentials
PASSWORD_PATHS=${PATH}/passwords
```

### Using Git with environment variables
Its would be pointless to hide crucial credentials in the `.env` file and push the file to git.

When commiting your code to your Git repository, you can ignore the `.env` file by adding it to your `.gitignore`.

A local `.gitignore` file is placed in the root directory of the project/Program. 

One Can also create a global file where any entry to that file will be ignored in all of your Git repositories.

To create a local `.gitignore` file, create a text file named `.gitignore`.

You can now list the file(s) or folder(s) that you would wish Git to ignore.

Example of a `.gitignore` file:

```
# used to add comments
# Ignore passwords folder
passwords

# Ignore all the text files
*.txt

# Ignore our credentials
.env
```
