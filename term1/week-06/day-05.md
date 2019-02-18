# Day 05 — Rails controllers & routing
## Outcomes
Students to understand **crud** (create, read, update, destroy) in rails controllers. How to setup and route to their own controller. How to connect data from a database to a controller. How to pass down data to the views. Further explore routes.rb file

## On successful completion of this unit students will be able to:
- generate a controller with scaffold
- create a controller from scratch
- have the model pass information to the controller
- have the controller pass information to the view
- re-route a route to the controller

## Guided instructions

## Resources

### Controllers
- demonstrate ```rails generate controller``` command
- create methods ```new create show edit update destroy``` when required
- discuss routing
- idea is to show how each method one after another
    - design new (new record) method
    - design the create method
    - design show method
    - design the edit method
    - design the update method
    - finally add the destroy method
- explore parameters from the form
- discuss and demonstrate safe/strong parameters
- discuss sessions
    - in cookies (user)
    - in cache (server)
    - in a database (MemCache, Redis)
- configure cookie session
- store/access session (user id)
- store/retrieve information from cookies
- explore flash (:notice, :alert, :flash)
- rendering html/json/xml using the ```respond_to``` method
- controller filters ```before_action```, ```after_action```, ```skip_before_action```

### Routes
- discuss crud in routing
- discuss and demonstrate routing
- discuss and demonstrate nested routing
- display routes using ```rails routes```


## Resources 
[Controllers](http://guides.rubyonrails.org/action_controller_overview.html)
[Routing](http://guides.rubyonrails.org/routing.html)