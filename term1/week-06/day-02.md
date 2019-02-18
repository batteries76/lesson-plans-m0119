# Day 02 — Rails scaffold & seeding
## Outcomes
Students to understand basic commands to scaffold rails application quickly and seed data into a database

## On successful completion of this unit students will be able to:
- run a rails scaffold command to generate a model, view and controller
- seed database with seed.rb

## Guided instructions
Repeating instructions from previous days helps students memorize commands
- generate a homepage ```rails generate controller Welcome index
- set root to Welcome page in routes.rb
- generate new rails app ```rails new shoppy```
- generate scaffold ```rails generate scaffold Product name description:text price:decimal brand```
- discuss migrations in rails
- run migrations ```rails db:migrate```
- discuss seeding a database
- code seed info with seeds.rb in db folder
```ruby
# prices in cents
products = [
    {
        name: 'Ryobi 12V 1.3Ah Drill Driver Kit',
        brand: 'Ryobi',
        description: 'The 12V Drill Driver Kit is your go to for all those small jobs around the home. With a compact design, built in LED light and 22 setting configurable clutch, this handy drill will help you tackle those odd jobs around your home.',
        price: 8900
    },
    {
        name: 'Makita 185mm 1200W Corded Circular Saw',
        brand: 'Makita',
        description: 'The Makita 185mm Circular Saw is ideal for any task and includes two 185mm saw blades for use with its high powered 1200W motor. ',
        price: 10900
    },
    {
        name: 'Tuscan Path 46cm Half Barrel Wooden Planter',
        brand: 'Tuscan Path',
        description: 'Tuscan Path’s Wooden Planters offer a multi-purpose planter with lots of natural, rustic character. Their authentic, simple design brings out the beauty of their wooden construction. Made from acacia, they are useful as storage, craft containers gift hampers and even as a cooler.',
        price: 4500
    },
    {
        name: 'Verve Design Chrome Hector Desk Lamp',
        brand: 'Verve Design',
        description: 'With a classic, retro feel the Hector desk lamp will look great on a desk, tabletop or bedside table. The adjustable shade makes it a practical and stylish lighting solution.',
        price: 4990
    }
]
# .create will not throw an error if seed fails
# .create! will throw an error if seed fails
Product.create!(products) { |product| puts "#{product[:name]} seeded" }
```
- run seed ```rails db:seed```
- view different pages for Products
- run ```rails routes``` to discuss routing paths and conventions

## Challenges
Students are to take a CSV file with headers unlike that of the table they are to create. They are to import the csv and map the csv headers to the appropriate table fields using the seed.rb file.


## Resources
- [Rails CLI](http://guides.rubyonrails.org/command_line.html)
- [Model callbacks](http://guides.rubyonrails.org/active_record_callbacks.html)