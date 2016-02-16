# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   For now, we'll use the `rails-api` gem to create rails applications.
    `rails-api` is set to become part of Rails 5. We will never type `rails
    new`, instead preferring `rails-api new`.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
The model layer is the hard working number cruncher in Rails that nobody sees. The controller layer sends data to the model layer and the model layer takes the request, processes it in the back end and spits out a response to the request back at the controller.
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller layer is the middle man between the model layer and the browser. It takes a request sent by the browser and sends it to the model layer in language that the model layer can easily work with. The model processes and sends data back to the controller which then makes the data easily readable on the browser for the user. It's the mastermind behind the scenes making everyone's job easier without them knowing it.
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
The router is the doorman of the MVC. It looks at the HTTP verb from the browser and determines the next steps that need to be taken. A simple yet incredibly essential piece to the request-response process in Rails.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
The client makes a GET request from the browser. The web server chooses the correct route for that request and sends the information to the controller layer. The controller layer takes that info and makes it so the model layer can read it and process it. The model layer controls the request in the back end and if all goes well, spits the confirmed info back into the controller layer which processes and sends the appropriate response to the server and browser. 
```
