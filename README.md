## About The Project
A very basic cloud-formation template to showcase sns-sqs fanout with an alarm on queue depth


### Prerequisites

* aws-cli installed
* aws-cli configured with an aws account with enough privileges to create the required resources


## Usage

### Set phone number for alerts
Update the parameters.json file to include phone number to receive alerts

### Create Stack
```
aws cloudformation create-stack --stack-name "s3-event-fanout"  --template-body file://template.yaml --parameters file://parameters.json
```

### Update Stack
```
aws cloudformation update-stack --stack-name "s3-event-fanout"  --template-body file://template.yaml --parameters file://parameters.json
```

### Delete stack
```
aws cloudformation delete-stack --stack-name "s3-event-fanout"
```

## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Project Link: [https://github.com/kalkirose/s3-event-fanout](https://github.com/kalkirose/s3-event-fanout)
