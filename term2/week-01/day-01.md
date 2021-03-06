# Day 01 — Authorization, devise and partials
## Outcomes
Students to have an understanding of Authentication in a web application (as apposed to Authorization). Students to have an understanding of HTML partials in Rails.

## On successful completion of this unit students will be able to:
- Create a user model using devise
- Have a user login to a website
- Have a user logout of a website
- Render a partial on a page

## Guided instructions

### Devise
- discuss authentication (vs authorization)
- guide students through the devise github page and wiki
- create a new rails project ```rails new instagram```
- install devise gem and bundle into rails project
- install devise scripts
- create user model ```rails g devise User```
- discuss migration file generated by devise
- discuss User model generated by devise
- discuss user routes generated by devise ```rails routes```
- migrate user model
- generate a welcome page ```rails g scaffold Pages welcome```
- add authentication to the application controller ```before_action :authenticate_user!```
- demo a user registration
- demo without authentication sign-in/sign-out links
- add sign-out to navigation bar
- add sign-in to navigation bar
- scaffold images ```rails g scaffold Image image_data:text description:text user:references```
- add to the create controller the user to the created image
```ruby
def create
    @image = Image.new(image_params)
    @image.user = current_user
...
```
- display user email on photo show page


## Partials
- add a partial file
- render the navbar with authentication links in the layout file

## Resources
- [Sessions in Rails](https://www.justinweiss.com/articles/how-rails-sessions-work/)
- [Devise](https://github.com/plataformatec/devise)
- [Devise getting started](https://github.com/plataformatec/devise#getting-started)
- [Devise sign-in/sign-out](https://github.com/plataformatec/devise/wiki/How-To:-Add-sign_in,-sign_out,-and-sign_up-links-to-your-layout-template)
- [Rails partials](http://guides.rubyonrails.org/layouts_and_rendering.html)
- [render method](https://apidock.com/rails/ActionController/Base/render)