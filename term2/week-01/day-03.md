# Day 03 — Geocoding
## Outcomes
Students to be able to geolocate a user based on user address information and in turn create a profile page

## On successful completion of this unit students will be able to:
- generate a login with devise
- generate a profile page with address details
- obtain longitude and latitude from address using geocoding
- display map on profile page of location

## Guided Instructions
- create a User model using devise
- create a welcome page
- generate a profile scaffold ```rails g scaffold Profile first_name last_name user:references address city country_code latitude:decimal longitude:decimal```
- create ```'/profile'``` routes for new, edit, create and show
- redirect a logged in user to a edit/new profile page if the user has no profile 
- add a method to the profile model that creates a full address
```ruby
def full_address
    "#{address}, #{city}, #{postcode},#{country_code}"
end
```
- add geocode gem and bundle install ```gem 'geocoder'```
- geocode the profile model 
```ruby
geocoded_by: :full_address
after_validation :geocode
```
- display a pinned map on the profile show page using longitude & latitude (suggest making a helper)

## Challenges
- create tests for model methods
- create tests for controller methods

## Resources
- [geocoder gem](http://www.rubygeocoder.com/)
- [country_select gem](https://github.com/stefanpenner/country_select)