## sequential iron-ajax calling example

Demonstrating weird behavior when triggering a second ajax request within the response handler of a first one. The
response handler of the second request is never actually triggered, it's actually the response handler of the first
ajax request that gets triggered , leading to recursive requests to ajax2.

`npm install && ./node_modules/.bin/bower install && ./node_modules/.bin/polyserve -p 8081`

Then hit up http://localhost:8081/components/iron-ajax-sequence/index.html

![sample output](https://raw.github.com/pdelanauze/iron-ajax-sequence/master/output.png)