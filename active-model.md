# Active Model
## Validation
1. options

1.1. validates_presence_of

``` rails
    validates_presence_of :name 
```

1.2. validates_numbericality_of

e.g. validates_numbericality_of :total

1.3. validates_uniqueness_of

e.g. validates_uniqueness_of :username

1.4 validates_confirmation_of

e.g. validates_confirmation_of :password

1.5 validates_acceptance_of

validates_acceptance_of :terms_of_service

1.6 validates_lenght_of :property, minimum: number, maximum: number

e.g validates_lenght_of :description, minimum: 50, maximum: 250

1.7 validates_format_of :property, with: /regex/i

e.g validates_format_of :email, with: /[a-z0-9]{3,100}@[a-z0-9]\.com/i

1.8 validates_inclusion_of

e.g validates_inclusion_of :year, in: 2010..2050

1.9 validates_exclusion_of

e.g validates_exclusion_of :year, in: 1990..2000,
    message: "Year was in the past!"

2. Alternative syntax

2.1. validates_<option>_of :<attribute>

e.g. validates_presence_of :name

2.2. validates :<attribute>, <option>:<value>[, <option>:<value>]

- Available from rails 3.0

e.g. validates :name, presense: true, length: { minimum: 10 }

3. Ref

[Active Model Validation APIs](http://apidock.com/rails/v3.0.0/ActiveModel/Validations/ClassMethods/validates)
