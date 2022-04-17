# Config APIs
Testing the API for getting server configuration. The API should always return the correct corresponding configuration with no exceptions.

## Get server configuration `GET /config`

Start server with the any `configs.json`. The API should return exactly the same thing.
| param | output |
| -- | -- |
| N/A | Exactly the same content as in `configs.json`, i.e. `{"weight_to_load": "resnet-18.pth", "model_arch": "resnet-18-32x32", "device": "cpu",     "pre_trained": False, "batch_size": 16, "shuffle": True, "num_workers": 8, "image_size": 32, "image_padding": "none", "num_classes": 9 }` |