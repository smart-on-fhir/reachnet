For this demo we will use HTTP-Server, a Node.js command line
static HTTP server, to serve the sample apps on “localhost”.

Download and install Node.js from https://nodejs.org/en/download/

To install HTTP-Server, use the following command (in the console):

```
npm install http-server -g
```

This demo contains three different sample apps. The `patient` app
demonstrates the basic structure of a single-patient SMART app. The
`population` SMART app illustrates population-level FHIR queries.
Finally, the `summary` SMART app provides a working example of
an app that displays a patient summary view.

To run a sample app, start HTTP-Server in the root directory of the app
(For convenience, we have provided shell scripts for you to use named
`runserver.sh` and `runserver.bat`. Use the one appropriate for your OS).

Now open a browser window and launch the app against one of the available
SMART-on-FHIR servers. Here is an example URL to use for launching an app
against the SMART-on-FHIR sandbox:

[http://localhost:8000/fhir-app/launch.html?iss=https://fhir-api-dstu2.smarthealthit.org](http://localhost:8000/fhir-app/launch.html?iss=https://fhir-api-dstu2.smarthealthit.org)

It is also possible to launch the sample apps against an open SMART
endpoint which does not require authentication. However, you will need
to know the identifier of the patient that you want to feed into the
app ahead of time. Here is an example against the SMART-on-FHIR sandbox:

[http://localhost:8000/fhir-app/launch.html?fhirServiceUrl=https://fhir-open-api-dstu2.smarthealthit.org&patientId=99912345](http://localhost:8000/fhir-app/launch.html?iss=https://fhir-api-dstu2.smarthealthit.org)

Another open endpoint to try would be `https://fhir.i2b2.org/srv-dstu2-0.3/api/open`
(patient ID `1000000005`)

Additional sample apps are available at https://github.com/smart-on-fhir/sample-apps
