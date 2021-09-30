# challenge-2-metadata

NXLog reads from a generic file with im_file. In the Output block, the xm_python python_call() procedure is used to execute the get_attribute() Python function, which adds one or more metadata fields to the event record. The output is then converted to JSON format and written to a file.


Google Compute Engine
The Google Cloud metadata server is available at metadata.google.internal. It is necessary to provide the header Metadata-Flavor: Google in order to get the response. For example, the request below retrieves the instance ID:

$ curl -H "Metadata-Flavor: Google" \
  "http://metadata.google.internal/computeMetadata/v1/instance/id"
