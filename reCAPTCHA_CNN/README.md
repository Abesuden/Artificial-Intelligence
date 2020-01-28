# reCAPTCHA CNN

## Getting Started


## Prerequisites

To run the code, you need the following installed:

 * python3
 * pip
 * python venv
 * The python libraries listed in requirements.txt

Follow these steps if you are new to this:

Install python3 and python3's package manager pip
```
sudo apt update
sudo apt install python3
sudo apt install python3-pip
python3 -m pip install --user virtualenv
```

Create a python virtual enviornment to install the dependencies
```
python3 -m venv .venv
```

Enter the virtual environment
```
source .venv/bin/activate
```

Install dependencies
```
pip install -r requirements.txt
```

## Deployment

Follow these steps once the virtual environment is set up:

### Step 1: Extract single letters from reCAPTCHA images

```
python3 extract_single_letters_from_captchas.py
```
*The results will be stored in the "extracted_letter_images" folder.*


### Step 2: Train the neural network to recognize single letters

```
python3 train_model.py
```
*This will write out "captcha_model.hdf5" and "model_labels.dat"*

## Versioning

I used [Git](https://git-scm.com/doc) for versioning. For the versions available, see the [tags on this repository](https://github.com/artificiall-intelligence/tags).

## Authors

* **Alex Besuden** - *constructed README* - [@abesuden](https://github.com/abesuden)

See also the list of [contributors](https://github.com/abesuden/artificial-intelligence/contributors) who participated in this project.

## License

This project is licensed under the [MIT](LICENSE.md) Creative Commons License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* [@Alex Besuden](https://github.com/abesuden) (**Virtual Environments**)
* [Adam Geitgey](https://github.com/ageitgey) (**Created Project**)
* Project was pulled from [here](https://medium.com/@ageitgey/how-to-break-a-captcha-system-in-15-minutes-with-machine-learning-dbebb035a710)*



