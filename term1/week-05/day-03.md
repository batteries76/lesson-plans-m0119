# Day 03 — HTTP Server & CSS Test
## Outcomes
Students to have a basic understanding of how a computer sends and receives http requests using a Rack or Webrick server.
Students to see how to include a web module into their server

## On successful completion of this unit students will be able to:
- create a minimal web server
- handle a http GET & POST request
- add a web module (i.e. Stripe)
- serve up a HTML document
- embed ERB into a HTML document
- handle a charge/payment using a web module (i.e. Stripe)
- learn about environment variables

## Guided instructions

### Stripe & main.rb
- build a basic ruby main.rb file that imports Stripe
- Configures Stripe using environment variables
- create a Stripe charge
- discuss Stripe
Explain to students the missing part ("tok_amex" token which is missing) and that this is in test mode
- store the charge in a variable
- retrieve a Stripe charge and print to screen

### Stripe & server.rb
- build a basic server.rb file that imports and configures a Webrick server
    - create a Routes using ```WEBrick::HTTPServlet::AbstractServlet```
    - create a basic Webrick gets route that responds with basic text
    - create a basic index.html file with HTML 5 code
    - load HTML file into server.rb using File class
    - explain ERB
    - add ERB to HTML file and embed Stripe key
- explain Stripe forms [Stripe Quickstart](https://stripe.com/docs/quickstart)

### CSS Test
- have students complete the CSS Test

## Challenges

## Resources
[Webrick](https://ruby-doc.org/stdlib-2.4.1/libdoc/webrick/rdoc/WEBrick.html)
[Stripe Gem](https://github.com/stripe/stripe-ruby)
[HTTP METHODS](https://restful-api-design.readthedocs.io/en/latest/methods.html)