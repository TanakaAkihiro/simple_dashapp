# Simple Dash app

This is a simple [Dash](https://dash.plotly.com/) app for dockerization.

## Installation & Running

Install dependencies by running

`pip install -r requirements.txt`

Start running the app with

`gunicorn -b 0.0.0.0:8050 --reload app:server`

or

`python3 app.py`

## Run with docker

Build the image:

`docker build . -t simple-dash`

Run a container:

`docker run -p 8050:8050 simple-dash`
