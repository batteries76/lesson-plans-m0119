# Day 05 — Authentication, Pundit gem
## Outcomes
Students to have an understanding of Authorization in a web application (as apposed to Authentication). 

## On successful completion of this unit students will be able to:
- Prevent users from viewing page content that is not authorized to them

## Guided instructions

gems:
```ruby
gem 'devise'
gem 'pundit'
gem "font-awesome-rails"
```

## Pundit
- discuss authorization
- discuss pundit gem
- demo pundit installtion
- ```gem "pundit"```
- ```bundle install && rails g pundit:install```
- create a user model using devise
- scaffold an Image model etc
- create a policy file ```image_prolicy.rb``` under app/policies
```ruby
     #suggested policies
        def show?
            user == image.user
        end

        def index?
            user.admin?
        end
```
- add ```authorize @image``` to show method
- visit & demo an image show page with different logged in users (this should result in authorization)

## likes
- create a join table between users and images called likes ```rails g migration CreateJoinTableLikes image user```
- modify migration file to give table name ```likes```
- add a join table relationship to the image model
```ruby
  has_and_belongs_to_many :likers, class_name: 'User', join_table: :likes
```
- create a method in the model that checks if the user has "liked" a photo
- create a toggle for liking a image in image model
- add a member route "like" to image route resources
- add the like action to the images controller
- add a like form to the show page view
- ensure authorization
- demo like/unlike actions
- decorate button with fontawesome gem

## Resources
- [Adding member routes](http://guides.rubyonrails.org/routing.html#adding-member-routes)
- [Nesting resources](http://weblog.jamisbuck.org/2007/2/5/nesting-resources)
- [pundit gem](https://github.com/varvet/pundit)
- [Join tables](http://edgeguides.rubyonrails.org/active_record_migrations.html#creating-a-table)
- [font awesome heart](https://fontawesome.com/icons/heart?style=solid)
- [font awesome heart empty](https://fontawesome.com/icons/heart?style=regular)
- [helpful font-awsome link](https://github.com/FortAwesome/Font-Awesome/wiki/Upgrading-from-3.2.1-to-4)