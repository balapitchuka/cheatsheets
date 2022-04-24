## Usage

     curl -k https://example.com           # Ignore SSL errors
     curl -s https://example.com           # Silence curl download infos, just content
     
     curl -X PUT --data-binary @myinput.json https://example.com/api/v1/endpoint     # use data from file
     
     # POST with data
     curl -XPOST --data-binary @myinput.txt       https://example.com/api
     curl -d '{ "key": "value", "some": "json" }' https://example.com/api
     curl -d 'param=key&param=key'                https://example.com/api     # application/x-www-form-urlencoded
     
     # HEAD request
     curl -I https://example.com/file
