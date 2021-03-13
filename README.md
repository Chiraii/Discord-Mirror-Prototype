# DuplicaDetector

## Installation

> pip3 install DuplicaDetector

## Information

- You'll need to create a folder called "pictures" (will be able to rename later) to save the pictures you upload to the lib.;
- DuplicaDetector will create a file called "db.pkl", it is the database it's using. If you want to *start over* you can just delete it or rename it

## Usage

### Import

> from DuplicaDetector import ImageChecker

> im = ImageChecker()

**OR**
> import DuplicaDetector as dd

> im = dd.ImageChecker()

**OR**
> import DuplicaDetector

> im = DuplicaDetector.ImageChecker()

### Check if an image is in database - DoesExist()
This function will check if the image already exist in the database by checking multiple values

##### Call
> im = ImageChecker()
> im.DoesExist("path_to_the_image")

#### Return
DoesExist returns an object with two values callable as method:
- ***path***

Gives the path to the image as a string
> im.DoesExist("path_to_the_image").path
-> "path_to_image"

- ***exists***

Tells if the image already existed or if it has been created as a boolean
> im.DoesExist("path_to_the_image").exists
-> True

### Exit - Exit()
The Exit() function saves the database

#### Call
> im = ImageChecker()

> im.Exit()

#### Return
The Exit() function does not return anything

## License
**MIT**