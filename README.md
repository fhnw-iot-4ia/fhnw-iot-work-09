# IoT Engineering
## Hands-on of lesson 9
For slides and example code, see [lesson 9](../../../fhnw-iot/blob/master/09/README.md)

> *Note: Do not work on this repository right away.*<br/>
> *[Create your personal copy by clicking this GitHub Classroom link](https://classroom.github.com/a/OeVLRv5T).*

### a) Dashboard as a service, 15'
* Choose a dashboard service and a transport protocol.
* Check the API docs to understand the payload format.
* Send data "as a device" with curl or with the mqtt CLI.
* The CLI runs on the Raspberry Pi or on your laptop.

### b) Glue code, 15'
* Configure & run the above TTN/ThingSpeak glue code.
* Host the code on the Raspberry Pi and on Zeit Now.
* Use curl to simulate calls from the TTN backend:<pre>
$ curl -v http://127.0.0.1:8080/ --data '{"app_id":"fhnw-iot","dev_id":"fhnw-iot-arduino-1","payload_raw": "FwAqAA=="}' # Base64</pre>
* Replace 127.0.0.1:8080 with your Zeit Now URL.

### c) Docker hosted dashboard, 15'
* Install Docker on your computer (not Raspberry Pi).
* Run InfluxDB and run/create a Grafana dashboard.
* Run Telegraf to get data from test.mosquitto.org.
* Send data "as a device" with mqtt, to Mosquitto.

### Submitting results
* [Commit and push](#git) local changes to your repository.
* Want a review? [Create an issue](../../issues/new), mention me (@tamberg).

## Tools
### Git
On your computer
* In the hands-on repository [fork for your class](../../network/members), in README.md, click the _GitHub Classroom link_.
* Once you accept the assessment, you get a personal, private repository URL for your _USER_NAME_:<pre>
http://github.com/fhnw-iot-CLASS/fhnw-iot-work-09-USER_NAME</pre>

On your computer or Raspberry Pi
* Clone the repository<pre>
    $ cd ~
    $ git clone REPO_URL</pre>
* Add a file<pre>
    $ git add FILE</pre>
* Commit changes<pre>
    $ git commit FILE -m "Fixed all bugs"</pre>
* Push changes<pre>
    $ git push</pre>

## Wiki
- [IoT Engineering Wiki](https://github.com/tamberg/fhnw-iot/wiki)

## Support
- [IoT Engineering Slack](https://fhnw-iot.slack.com/)
