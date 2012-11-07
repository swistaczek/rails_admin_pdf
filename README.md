RailsAdminPdf Gem (Engine)
========

PDF Builder for RailsAdmin.

Installation
========

* Add to Gemfile and bundle install:
```ruby
gem "rails_admin_pdf", :git => "git://github.com/stephskardal/rails_admin_pdf.git"
```

* Register in initializers/rails_admin.rb

```ruby
RailsAdmin.config do |config|

  config.actions do
    dashboard
    index
    new
    show
    pdf
    edit
    delete
  end

  #...
end
```

* Add prawn to your main application, and create "#{class}Report" for every class that you would like to export.

* If applicable, add right to :pdf action in CanCan ability class


Copyright
========

Copyright (c) 2012 End Point & Steph Skardal. 
