# RPS_Game

## Prerequisites

Install python version 3.x (for example using Anaconda).

## Setup

some instructions here

1. Clone [the repo](https://github.com/Lhceddie1104/RPS_Game) from GitHub, and put it somewhere (like your Desktop).
2. Navigate to the local repo from the command line (for example if on your desktop):

```sh
cd ~/Desktop/my-first-app-fall-2026
```

3. Create a new Anaconda virtual environment called "rps-env" (first time only):

```sh
conda create -n rps-env python=3.11
```

4. Activate the virtual environment as necessary (every time you come back to the project):

```sh
conda activate rps-env
```

5. Install package dependencies:

```sh
pip3 install -r requirements.txt
```

## Configuration

The stocks functionality requires an AlphaVantage API key. Obtain a premium AlphaVantage API Key (using the [form](https://www.alphavantage.co/support/#api-key) or shared by the prof).

Create a local ".env" file and store your environment variable in there:

```sh
# this is the ".env" file...

ALPHAVANTAGE_API_KEY="______________"
```

## Usage

### Command Line App

Run the example script:

```sh
python3 app/my_script.py

# alternatively:
python3 -m app.my_script
```


Run the example script:

```sh
python3 app/rps.py

# alternatively:
python3 -m app.rps
```

Stocks dashboard:

```sh
python3 -m app.stocks
```

### Web App

To run the web app:

```sh
# if we have the FLASK_APP=web_app env var in the ".env" file:
flask run

# Mac OS:
FLASK_APP=web_app python3 -m flask run

# Windows OS:
# ... if `export` doesn't work for you, try `set` instead
# ... or set FLASK_APP variable via ".env" file
export FLASK_APP=web_app
flask run
```
To stop the local web server while it is running, press "control+c" from the termal.

## Testing

To run tests:

```sh
pytest
```
