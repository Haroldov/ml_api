# Machine Learning Manager System Using FastAPI & Rest

This is a manager system using rest to build create, train and predict models stored in a relational database.

# How To Run

First make sure you have poetry installed. Then:

```sh
$ poetry run python app/app.py
```

Or with docker do:

```sh
$ docker-compose up
```

# Available Endpoints

* `POST /models`: Creates a model with the specified parameters in the body.
Example body:

```json
{
  "model": "MLPClassifier",
  "params": {
    "alpha": 0.0001,
    "hidden_layer_sizes": 20
  },
  "num_features": 4,
  "num_classes": 2
}
```