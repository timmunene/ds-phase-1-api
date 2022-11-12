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
