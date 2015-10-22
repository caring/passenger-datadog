# passenger-datadog

Inspired by [passengeri-datadog-monitor](https://github.com/Sjeanpierre/passenger-datadog-monitor)

This gem can be used to send stats from Passenger to Datadog. It makes use of
the command `passenger-status`, and the Ruby implementation of `statsd`
provided by [dogstatsd-ruby](https://github.com/DataDog/dogstatsd-ruby))

In order to gather stats on all Passenger instances, Passenger recommends
running `passenger-status` as `root`. Therefore, it is recommended that
`passenger_datadog` be run as `root` as well. `passenger_datadog` will also
work if run as the same user that is used to run the application in Passenger.

If running `passenger_datadog` as a user other than the user that owns the application
in Passenger, make sure that same version of Passenger is installed for both users.

## Installation
```
$ gem install passenger_datadog
```

## Usage

### Typical Usage
```
$ passenger-datadog [start|stop|restart|status]
```

### Help
```
$ passenger-datadog
```
or
```
$ passenger-datadog [-h|--help]
```
