# bxlogic
Binary eXperimental LOGistics Integration and Control

BXLOGIC allows a single Dispatcher to coordinate the efforts of a team of Couriers. The Dispatcher interacts with the system via a web interface (a series of forms), and the Couriers interact with the system via SMS. The stack currently uses Twilio to forward SMS traffic to one of our web endpoints.

## Getting Started

A live BXL stack consists of the following processes:

- web listener, started by the `make run` target
- event queue consumer, started by the `make qscan` target
- job-data queue consumer, started by the `make qlisten` target

### Prerequisites

Install the dependencies by issuing `pipenv install`. `pipenv shell` will start the virtual environment.
This project also requires access to the following services:

- PostgreSQL v9.5 or greater
- S3 object storage
- two SQS queues configured on AWS: one for job data, one for out-of-band event data


### Installing


## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Flask](http://www.dropwizard.io/1.0.2/docs/) - Pythonic web framework
* [SNAP](https://maven.apache.org/) - wrapper around Flask
* [SqlAlchemy](https://rometools.github.io/rome/) - Object -Relational Mapping 

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors

* **Dexter Taylor** 

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used

